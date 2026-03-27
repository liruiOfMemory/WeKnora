<template>
    <div class="dialogue-wrap">
        <div class="dialogue-answers">
            <!-- <div class="dialogue-title">
                <span>{{ $t('createChat.title') }}</span>
            </div> -->
            <div class="ai-title-container">
                <div class="decorative-circle floating"></div>
                <div class="decorative-circle-2 floating" style="animation-delay: -4s;"></div>

                <div class="title-content">
                    <h1 class="main-title fade-in-up">智析数据 · 洞见未来</h1>
                    <br/>
                    <p class="subtitle fade-in-up" style="animation-delay: 0.2s;">AI数据智能分析平台</p>

                    <div class="tagline fade-in-up" style="animation-delay: 0.4s;">
                        基于<span class="highlight">大数据分析</span>与<span class="highlight">人工智能算法</span>，
                        深度解析数据趋势，提供精准决策支持与未来洞察，
                        构建智能化管理体系。
                    </div>
                </div>
            </div>
            <InputField @send-msg="sendMsg"></InputField>
        </div>
    </div>

    <!-- 知识库编辑器（创建/编辑统一组件） -->
    <KnowledgeBaseEditorModal
      :visible="uiStore.showKBEditorModal"
      :mode="uiStore.kbEditorMode"
      :kb-id="uiStore.currentKBId || undefined"
      :initial-type="uiStore.kbEditorType"
      @update:visible="(val) => val ? null : uiStore.closeKBEditor()"
      @success="handleKBEditorSuccess"
    />
</template>
<script setup lang="ts">
import { ref } from 'vue';
import InputField from '@/components/Input-field.vue';
import { createSessions } from "@/api/chat/index";
import { useMenuStore } from '@/stores/menu';
import { useSettingsStore } from '@/stores/settings';
import { useUIStore } from '@/stores/ui';
import { useRoute, useRouter } from 'vue-router';
import { MessagePlugin } from 'tdesign-vue-next';
import { useI18n } from 'vue-i18n';
import KnowledgeBaseEditorModal from '@/views/knowledge/KnowledgeBaseEditorModal.vue';
import { useKnowledgeBaseCreationNavigation } from '@/hooks/useKnowledgeBaseCreationNavigation';

const router = useRouter();
const route = useRoute();
const usemenuStore = useMenuStore();
const settingsStore = useSettingsStore();
const uiStore = useUIStore();
const { t } = useI18n();
const { navigateToKnowledgeBaseList } = useKnowledgeBaseCreationNavigation();

const sendMsg = (value: string, modelId: string, mentionedItems: any[], imageFiles: any[] = []) => {
    createNewSession(value, modelId, mentionedItems, imageFiles);
}

async function createNewSession(value: string, modelId: string, mentionedItems: any[] = [], imageFiles: any[] = []) {
    const selectedKbs = settingsStore.settings.selectedKnowledgeBases || [];
    const selectedFiles = settingsStore.settings.selectedFiles || [];

    // 构建 session 数据，包含 Agent 配置
    const sessionData: any = {};

    // 添加 Agent 配置（知识库信息在 agent_config 中）
    sessionData.agent_config = {
        enabled: true,
        max_iterations: settingsStore.agentConfig.maxIterations,
        temperature: settingsStore.agentConfig.temperature,
        knowledge_bases: selectedKbs,  // 所有选中的知识库
        knowledge_ids: selectedFiles,  // 所有选中的普通知识/文件
        allowed_tools: settingsStore.agentConfig.allowedTools
    };

    try {
        const res = await createSessions(sessionData);
        if (res.data && res.data.id) {
            await navigateToSession(res.data.id, value, modelId, mentionedItems, imageFiles);
        } else {
            console.error('[createChat] Failed to create session');
            MessagePlugin.error(t('createChat.messages.createFailed'));
        }
    } catch (error) {
        console.error('[createChat] Create session error:', error);
        MessagePlugin.error(t('createChat.messages.createError'));
    }
}

const navigateToSession = async (sessionId: string, value: string, modelId: string, mentionedItems: any[], imageFiles: any[] = []) => {
    const now = new Date().toISOString();
    let obj = {
        title: t('createChat.newSessionTitle'),
        path: `chat/${sessionId}`,
        id: sessionId,
        isMore: false,
        isNoTitle: true,
        created_at: now,
        updated_at: now
    };
    usemenuStore.updataMenuChildren(obj);
    usemenuStore.changeIsFirstSession(true);
    usemenuStore.changeFirstQuery(value, mentionedItems, modelId, imageFiles);
    router.push(`/platform/chat/${sessionId}`);
}

const handleKBEditorSuccess = (kbId: string) => {
    navigateToKnowledgeBaseList(kbId)
}

</script>
<style lang="less" scoped>
.dialogue-wrap {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
    // position: relative;
}

.dialogue-answers {
    position: absolute;
    display: flex;
    flex-flow: column;
    align-items: center;

    :deep(.answers-input) {
        position: static;
        transform: translateX(0);
    }
}

.dialogue-title {
    display: flex;
    color: var(--td-text-color-primary);
    font-family: "PingFang SC";
    font-size: 28px;
    font-weight: 600;
    align-items: center;
    margin-bottom: 30px;

    .icon {
        display: flex;
        width: 32px;
        height: 32px;
        justify-content: center;
        align-items: center;
        border-radius: 6px;
        background: var(--td-bg-color-container);
        box-shadow: var(--td-shadow-1);
        margin-right: 12px;

        .logo_img {
            height: 24px;
            width: 24px;
        }
    }
}

@media (max-width: 1250px) and (min-width: 1045px) {
    .answers-input {
        transform: translateX(-329px);
    }

    :deep(.t-textarea__inner) {
        width: 654px !important;
    }
}

@media (max-width: 1045px) {
    .answers-input {
        transform: translateX(-250px);
    }

    :deep(.t-textarea__inner) {
        width: 500px !important;
    }
}
@media (max-width: 750px) {
    .answers-input {
        transform: translateX(-250px);
    }

    :deep(.t-textarea__inner) {
        width: 340px !important;
    }
}
@media (max-width: 600px) {
    .answers-input {
        transform: translateX(-250px);
    }

    :deep(.t-textarea__inner) {
        width: 300px !important;
    }
}

</style>
<style lang="less">
.del-menu-popup {
    z-index: 99 !important;

    .t-popup__content {
        width: 100px;
        height: 40px;
        line-height: 30px;
        padding-left: 14px;
        cursor: pointer;
        margin-top: 4px !important;

    }
}
</style>
<style lang="less">
.ai-title-container {
    text-align: center;
    padding: 60px 80px;
    /* 移除白色背景，使用透明背景 */
    background: transparent;
    border-radius: 24px;
    /* 移除边框和内阴影 */
    box-shadow: none;
    position: relative;
    border: none;
    max-width: 800px;
    width: 100%;
    transition: all 0.3s ease;
}

.ai-title-container:hover {
    transform: translateY(-5px);
    /* 移除悬停时的阴影 */
    box-shadow: none;
}

.decorative-circle {
    position: absolute;
    width: 150px;
    height: 150px;
    background: linear-gradient(135deg, rgba(42, 109, 255, 0.08) 0%, rgba(0, 198, 255, 0.08) 100%);
    border-radius: 50%;
    top: 0px;
    left: -50px;
    z-index: 0;
}

.decorative-circle-2 {
    position: absolute;
    width: 100px;
    height: 100px;
    background: linear-gradient(135deg, rgba(42, 109, 255, 0.05) 0%, rgba(0, 198, 255, 0.05) 100%);
    border-radius: 50%;
    bottom: -40px;
    right: -40px;
    z-index: 0;
}

.title-content {
    position: relative;
    z-index: 1;
}

.main-title {
    font-size: 3rem;
    font-weight: 600;
    background: linear-gradient(135deg, #2A6DFF 0%, #00C6FF 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    letter-spacing: 1.2px;
    line-height: 1.2;
    margin-bottom: 20px;
    text-shadow: 0 2px 15px rgba(42, 109, 255, 0.15);
    position: relative;
    display: inline-block;
    padding: 0 15px;
}

.main-title::after {
    content: '';
    position: absolute;
    bottom: -12px;
    left: 15%;
    width: 70%;
    height: 3px;
    background: linear-gradient(90deg, transparent, #2A6DFF, transparent);
    border-radius: 2px;
}

.subtitle {
    font-size: 1.3rem;
    color: #555;
    font-weight: 400;
    margin-bottom: 40px;
    letter-spacing: 0.8px;
    position: relative;
    display: inline-block;
    padding: 0 20px;
}

.subtitle::before,
.subtitle::after {
    content: '✦';
    position: absolute;
    color: #2A6DFF;
    opacity: 0.6;
    font-size: 0.8em;
    top: 50%;
    transform: translateY(-50%);
}

.subtitle::before {
    left: 0;
}

.subtitle::after {
    right: 0;
}

.tagline {
    font-size: 1.1rem;
    color: #666;
    font-style: normal;
    line-height: 1.8;
    max-width: 600px;
    margin: 0 auto;
    padding: 30px 40px;
    background: linear-gradient(to right, rgba(42, 109, 255, 0.03), rgba(0, 198, 255, 0.03));
    border-radius: 16px;
    border: 1px solid rgba(42, 109, 255, 0.08);
    position: relative;
}

.tagline::before {
    content: '';
    position: absolute;
    top: -1px;
    left: -1px;
    right: -1px;
    bottom: -1px;
    background: linear-gradient(45deg, transparent, rgba(42, 109, 255, 0.05), transparent);
    border-radius: 16px;
    z-index: -1;
}

.highlight {
    color: #2A6DFF;
    font-weight: 500;
    position: relative;
}

.highlight::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 100%;
    height: 2px;
    background: linear-gradient(90deg, #2A6DFF, #00C6FF);
    opacity: 0.3;
    transition: opacity 0.3s ease;
}

.highlight:hover::after {
    opacity: 0.6;
}

/* 响应式设计 */
@media (max-width: 768px) {
    .ai-title-container {
        padding: 40px 30px;
        margin: 20px;
    }

    .main-title {
        font-size: 2.2rem;
    }

    .subtitle {
        font-size: 1.1rem;
    }

    .tagline {
        font-size: 1rem;
        padding: 25px 30px;
    }

    .decorative-circle {
        width: 100px;
        height: 100px;
        top: -30px;
        left: -30px;
    }

    .decorative-circle-2 {
        width: 70px;
        height: 70px;
        bottom: -25px;
        right: -25px;
    }
}

@media (max-width: 480px) {
    .main-title {
        font-size: 1.8rem;
    }

    .subtitle {
        font-size: 0.95rem;
    }

    .tagline {
        font-size: 0.95rem;
        padding: 20px 25px;
    }
}

/* 动画效果 */
@keyframes float {

    0%,
    100% {
        transform: translateY(0) rotate(0deg);
    }

    50% {
        transform: translateY(-10px) rotate(180deg);
    }
}

.floating {
    animation: float 8s ease-in-out infinite;
}

@keyframes fadeInUp {
    from {
        opacity: 0;
        transform: translateY(20px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.fade-in-up {
    animation: fadeInUp 0.8s ease-out;
}
</style>
