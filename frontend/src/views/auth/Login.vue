<template>
  <div class="login-layout">
    <!-- 背景装饰开始 -->
    <!-- 四方网格 -->
    <svg class="bg-net" viewBox="0 0 1440 900" preserveAspectRatio="xMidYMid slice" fill="none">
      <g stroke="rgba(110,231,183,.15)" stroke-width="1.2">
        <path class="net-dash" d="M120 640 L300 470 L520 560 L700 380 L920 470 L1130 300" />
        <path d="M300 470 L430 250 L700 380 M520 560 L640 720 L920 470 M700 380 L810 180 L1130 300" />
        <path class="net-dash" d="M430 250 L810 180" />
        <path d="M60 200 L230 320 L430 250 M1130 300 L1320 420 L1240 620" />
      </g>
      <g fill="rgba(110,231,183,.55)">
        <circle cx="300" cy="470" r="3.5" />
        <circle cx="700" cy="380" r="4.5" />
        <circle cx="920" cy="470" r="3" />
        <circle cx="1130" cy="300" r="4" />
        <circle cx="430" cy="250" r="3" />
        <circle cx="1240" cy="620" r="3.5" />
      </g>
      <g fill="rgba(52,211,153,.9)" class="float-a">
        <circle cx="520" cy="560" r="5" />
        <circle cx="810" cy="180" r="5" />
      </g>
      <g fill="rgba(209,250,229,.9)" class="float-b">
        <circle cx="640" cy="720" r="4" />
        <circle cx="1320" cy="420" r="4" />
      </g>
      <g fill="rgba(167,243,208,.4)">
        <circle cx="120" cy="640" r="2.5" />
        <circle cx="60" cy="200" r="2.5" />
        <circle cx="230" cy="320" r="2.5" />
        <circle cx="1020" cy="760" r="2.5" />
        <circle cx="1380" cy="160" r="2.5" />
        <circle cx="240" cy="820" r="2.5" />
      </g>
    </svg>
    <!-- 连接的轨道线 -->
    <div class="bg-grid"></div>
    <!-- 动的线条 -->
    <!-- <div class="glow glow-1"></div>
    <div class="glow glow-2"></div> -->
    <!-- 漂浮玻璃信息片（产品能力氛围） -->
    <div class="float-chip fc-1">
      <span class="fc-ic">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
          <path d="M18 8a6 6 0 0 0-12 0c0 7-3 9-3 9h18s-3-2-3-9" />
          <path d="M13.7 21a2 2 0 0 1-3.4 0" />
        </svg>
      </span>
      <span><b>AI 洞察</b> · 发现 3 条组合型风险线索</span>
    </div>
    <div class="float-chip fc-2">
      <span class="fc-ic">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
          <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z" />
          <path d="M14 2v6h6M9 15l2 2 4-4" />
        </svg>
      </span>
      <span><b>AI报告</b> ·《预算执行报告》已生成</span>
    </div>
    <!-- 背景装饰结束 -->
    <!-- 小云智问头部 -->
    <header class="topbar" style="padding: 0.5rem">
      <div class="brand">
        <span class="brand-mark">
          <svg width="19" height="19" viewBox="0 0 24 24" fill="#fff">
            <path d="M12 2l2.1 6.3L20 10l-5.9 1.7L12 18l-2.1-6.3L4 10l5.9-1.7L12 2z" />
            <circle cx="19" cy="18" r="2" />
          </svg>
        </span>
        <span class="brand-name">小云智问</span>
        <span class="brand-div"></span>
        <span class="brand-sub">云南省人大预算和国有资产联网监督系统</span>
      </div>
      <div class="net-chip">
        <svg width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
          <rect x="3" y="11" width="18" height="11" rx="2" />
          <path d="M7 11V7a5 5 0 0 1 10 0v4" />
        </svg>
        政务外网 · 安全接入
      </div>
    </header>
    <!-- 主要的内容 -->
    <div class="main-container" style="padding-top: 4rem">
      <!-- 左侧品牌区 -->
      <div class="hero" style="padding: 0.5rem">
        <div class="eyebrow">云南省人大预算和国有资产联网监督系统 | AI 智能助手</div>
        <!-- <h1><span class="grad">智析预算数据</span><span class="dot">·</span>洞见监督未来</h1>
        <p class="sub">以大模型深度赋能预算审查监督——<b>听得懂</b>问话、<b>看得见</b>关联、<b>主动提</b>风险、<b>学得会</b>逻辑，让“1 人 1 委”的县级人大也能高质量完成监督任务。</p> -->

        <div class="caps">
          <div class="cap">
            <span class="cap-ic"
              ><svg width="19" height="19" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
                <path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z" />
                <path d="M8 9h8M8 13h5" />
              </svg>
            </span>
            <div>
              <h3>智能问答与拓展分析</h3>
              <p>自然语言即问即答，自动关联数据维度，输出有分析、有结论的回答</p>
            </div>
          </div>
          <div class="cap">
            <span class="cap-ic" data-page-node-id="DZ4iaUh4Zh9fJVee9YKjUB"
              ><svg
                width="19"
                height="19"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="1.8"
                stroke-linecap="round"
                stroke-linejoin="round"
                data-page-node-id="7UwIjUVd7JqNm9sR601EzZ"
              >
                <path d="M16 3h5v5M21 3l-7 7M8 21H3v-5M3 21l7-7" data-page-node-id="DVBOfcP6EtaVRVRVxGOcVA" />
              </svg>
            </span>
            <div data-page-node-id="Kqncj43RqWCqqKxoyHZ8qJ">
              <h3 data-page-node-id="Nf7CTu6ApK8nBJ1mGOID7G">智能比对与综合分析</h3>
              <p data-page-node-id="sxZJDQxj3a0phDHWC66POc">多源数据自动比对，识别偏差、异常与趋势，输出有判断的综合研判</p>
            </div>
          </div>
          <div class="cap">
            <span class="cap-ic"
              ><svg width="19" height="19" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
                <path d="M12 2l8 4v6c0 5-3.5 8.5-8 10-4.5-1.5-8-5-8-10V6z" />
                <path d="M9 12l2 2 4-4" />
              </svg>
            </span>
            <div>
              <h3>规则触发 + AI 洞察</h3>
              <p>双层预警机制，在既有规则之上主动扫描，提炼高价值风险线索</p>
            </div>
          </div>
          <div class="cap">
            <span class="cap-ic"
              ><svg width="19" height="19" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8" stroke-linecap="round" stroke-linejoin="round">
                <path d="M12 20h9M16.5 3.5a2.1 2.1 0 0 1 3 3L7 19l-4 1 1-4z" data-page-node-id="Fo5PWVxADmcIQcy3v16hnO" />
              </svg>
            </span>
            <div>
              <h3>智能报告生成</h3>
              <p>学习历年监督稿件与监督逻辑，自动生成符合人大监督视角的报告</p>
            </div>
          </div>
        </div>
      </div>
      <div>
        <!-- Right Form Section -->
        <div class="form-section">
          <div class="form-panel">
            <!-- Login Card -->
            <div class="form-card" v-if="!isRegisterMode">
              <!-- invite_only 模式下共享链接停在登录卡，同样需要邀请上下文。 -->
              <div v-if="inviteLookup" class="invite-banner">
                <t-icon name="link" class="invite-banner__icon" />
                <div class="invite-banner__text">
                  <div class="invite-banner__title">
                    {{
                      $t("inviteRegister.bannerTitle", {
                        tenant: inviteLookup.tenant_name || "",
                      })
                    }}
                  </div>
                  <div class="invite-banner__hint">
                    {{ $t("inviteRegister.bannerHintLogin") }}
                  </div>
                </div>
              </div>
              <div v-else-if="inviteLookupError" class="invite-banner invite-banner--error">
                {{ inviteLookupError }}
              </div>
              <div class="form-header">
                <h2 class="form-title">{{ $t("auth.login") }}</h2>
                <p class="form-welcome">{{ $t("auth.subtitle") }}</p>
                <p v-if="registrationEnabled" class="form-hint">
                  {{ $t("auth.loginHint") }}
                </p>
              </div>

              <div class="form-content">
                <t-form ref="formRef" :data="formData" :rules="formRules" @submit="handleLogin" layout="vertical" label-align="top">
                  <t-form-item :label="$t('auth.email')" name="email">
                    <t-input v-model="formData.email" :placeholder="$t('auth.emailPlaceholder')" type="text" autocomplete="email" size="large" :disabled="loading" />
                  </t-form-item>

                  <t-form-item :label="$t('auth.password')" name="password">
                    <t-input
                      v-model="formData.password"
                      :placeholder="$t('auth.passwordPlaceholder')"
                      type="password"
                      autocomplete="current-password"
                      size="large"
                      :disabled="loading"
                      @enter="handleLogin"
                    />
                  </t-form-item>

                  <t-button type="submit" theme="primary" size="large" block :loading="loading" class="submit-button">
                    {{ loading ? $t("auth.loggingIn") : $t("auth.login") }}
                  </t-button>

                  <div class="register-cta" v-if="registrationEnabled">
                    <div class="register-cta__divider">
                      <span>{{ $t("auth.firstTime") }}</span>
                    </div>
                    <t-button theme="default" variant="outline" size="large" block class="register-cta__button" :disabled="loading" @click="toggleMode">
                      {{ $t("auth.createAccount") }}
                    </t-button>
                  </div>

                  <div v-if="oidcEnabled" class="oidc-divider">
                    <span>{{ $t("auth.orContinueWith") }}</span>
                  </div>

                  <t-button v-if="oidcEnabled" theme="default" size="large" block :loading="oidcLoading" :disabled="loading" class="oidc-button" @click="handleOIDCLogin">
                    {{ oidcLoading ? $t("auth.redirectingToOIDC") : oidcLoginText }}
                  </t-button>
                </t-form>

                <!-- Features list -->
                <div class="login-features">
                  <div class="feature-item">
                    <span class="feature-icon">✓</span>
                    <span class="feature-text">{{ $t("platform.multimodalParsing") }}</span>
                  </div>
                  <div class="feature-item">
                    <span class="feature-icon">✓</span>
                    <span class="feature-text">{{ $t("platform.hybridSearchEngine") }}</span>
                  </div>
                  <div class="feature-item">
                    <span class="feature-icon">✓</span>
                    <span class="feature-text">{{ $t("platform.ragQandA") }}</span>
                  </div>
                </div>
              </div>
            </div>

            <!-- Register Card. Renders when the user is in register mode
             AND either self-service registration is enabled OR they
             arrived with a valid share-link token (which bypasses the
             invite_only gate). -->
            <div class="form-card" v-if="isRegisterMode && (registrationEnabled || inviteLookup)">
              <!-- Share-link banner: shown only when ?token= resolved to a
               real invitation row. Sits above the form header so the
               invitee instantly sees who invited them and into which
               workspace, without bumping the existing register UX. -->
              <div v-if="inviteLookup" class="invite-banner">
                <t-icon name="link" class="invite-banner__icon" />
                <div class="invite-banner__text">
                  <div class="invite-banner__title">
                    {{
                      $t("inviteRegister.bannerTitle", {
                        tenant: inviteLookup.tenant_name || "",
                      })
                    }}
                  </div>
                  <div class="invite-banner__hint">
                    {{ $t("inviteRegister.bannerHint") }}
                  </div>
                </div>
              </div>
              <div v-else-if="inviteLookupError" class="invite-banner invite-banner--error">
                {{ inviteLookupError }}
              </div>
              <div class="form-header">
                <h2 class="form-title">{{ $t("auth.createAccount") }}</h2>
                <p class="form-subtitle">{{ $t("auth.registerSubtitle") }}</p>
              </div>

              <div class="form-content">
                <t-form ref="registerFormRef" :data="registerData" :rules="registerRules" @submit="handleRegister" layout="vertical" label-align="top">
                  <t-form-item :label="$t('auth.username')" name="username">
                    <t-input v-model="registerData.username" :placeholder="$t('auth.usernamePlaceholder')" size="large" :disabled="loading" />
                  </t-form-item>

                  <t-form-item :label="$t('auth.email')" name="email">
                    <t-input v-model="registerData.email" :placeholder="$t('auth.emailPlaceholder')" type="text" autocomplete="email" size="large" :disabled="loading" />
                  </t-form-item>

                  <t-form-item :label="$t('auth.password')" name="password">
                    <t-input v-model="registerData.password" :placeholder="$t('auth.passwordPlaceholder')" type="password" autocomplete="new-password" size="large" :disabled="loading" />
                  </t-form-item>

                  <t-form-item :label="$t('auth.confirmPassword')" name="confirmPassword">
                    <t-input
                      v-model="registerData.confirmPassword"
                      :placeholder="$t('auth.confirmPasswordPlaceholder')"
                      type="password"
                      autocomplete="new-password"
                      size="large"
                      :disabled="loading"
                      @enter="handleRegister"
                    />
                  </t-form-item>

                  <t-button type="submit" theme="primary" size="large" block :loading="loading" class="submit-button">
                    {{ loading ? $t("auth.registering") : $t("auth.register") }}
                  </t-button>
                </t-form>

                <div class="form-footer">
                  <span>{{ $t("auth.haveAccount") }}</span>
                  <a href="#" @click.prevent="toggleMode" class="link-button">
                    {{ $t("auth.backToLogin") }}
                  </a>
                </div>

                <!-- Features list for register -->
                <div class="login-features">
                  <div class="feature-item">
                    <span class="feature-icon">✓</span>
                    <span class="feature-text">{{ $t("platform.independentTenant") }}</span>
                  </div>
                  <div class="feature-item">
                    <span class="feature-icon">✓</span>
                    <span class="feature-text">{{ $t("platform.fullApiAccess") }}</span>
                  </div>
                  <div class="feature-item">
                    <span class="feature-icon">✓</span>
                    <span class="feature-text">{{ $t("platform.knowledgeBaseManagement") }}</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref, reactive, nextTick, onMounted, onBeforeUnmount, computed } from "vue";
import { useRoute, useRouter } from "vue-router";
import { MessagePlugin } from "tdesign-vue-next";
import { useRoleLabel } from "@/composables/useRoleLabel";
import { notifyLoginSuccess } from "@/utils/loginNotify";
import { Swiper, SwiperSlide } from "swiper/vue";
import { Autoplay, EffectFade, Pagination } from "swiper/modules";
import "swiper/css";
import "swiper/css/effect-fade";
import "swiper/css/pagination";
import { login, register, getOIDCAuthorizationURL, getOIDCConfig, autoSetup, getAuthConfig, userInfoFromApi, getInvitationByToken, registerByInvite, type InviteLookup } from "@/api/auth";
import { useAuthStore } from "@/stores/auth";
import { useI18n } from "vue-i18n";

// Import screenshot images
import screenshot1 from "@/assets/img/screenshot-1.svg";
import screenshot2 from "@/assets/img/screenshot-2.svg";
import screenshot3 from "@/assets/img/screenshot-3.svg";
import screenshot4 from "@/assets/img/screenshot-4.svg";

const router = useRouter();
const route = useRoute();
const authStore = useAuthStore();
const { t, tm, locale } = useI18n();
const { formatRole, roleIcon } = useRoleLabel();

// Swiper modules
const modules = [Autoplay, EffectFade, Pagination];

// Carousel slides data
const slides = [
  {
    image: screenshot4,
    title: t("platform.carousel.agenticRagTitle"),
    description: t("platform.carousel.agenticRagDesc"),
  },
  {
    image: screenshot2,
    title: t("platform.carousel.hybridSearchTitle"),
    description: t("platform.carousel.hybridSearchDesc"),
  },
  {
    image: screenshot3,
    title: t("platform.carousel.wikiTitle"),
    description: t("platform.carousel.wikiDesc"),
  },
  {
    image: screenshot1,
    title: t("platform.carousel.smartDocRetrievalTitle"),
    description: t("platform.carousel.smartDocRetrievalDesc"),
  },
];

// Form references
const formRef = ref();
const registerFormRef = ref();

// State management
const loading = ref(false);
const oidcLoading = ref(false);
const isRegisterMode = ref(false);
const showLanguageMenu = ref(false);
const oidcEnabled = ref(false);
const oidcProviderName = ref("");
// registrationEnabled defaults to true so that on first paint the Register
// link is visible; the actual mode is fetched from /auth/config in onMounted.
// In invite_only mode the link/card are hidden.
const registrationEnabled = ref(true);

// invite-link state. When the URL carries ?token=xxx we resolve it to
// the originating tenant + role and switch the form into a "register
// via invitation" mode. The token bypasses the normal invite_only
// gate — possessing it IS the authorisation. Submitting the register
// form with this set hits /auth/register-by-invite (auto-login on
// success) instead of /auth/register.
const inviteToken = ref("");
const inviteLookup = ref<InviteLookup | null>(null);
const inviteLookupError = ref("");
const inviteLookupLoading = ref(false);

// Language options
const languageOptions = [
  { value: "zh-CN", label: "简体中文", shortLabel: "中文", flag: "🇨🇳" },
  { value: "en-US", label: "English", shortLabel: "EN", flag: "🇺🇸" },
  { value: "ru-RU", label: "Русский", shortLabel: "RU", flag: "🇷🇺" },
  { value: "ko-KR", label: "한국어", shortLabel: "한국어", flag: "🇰🇷" },
];

const currentLanguage = computed(() => locale.value);
const oidcLoginText = computed(() => {
  if (oidcProviderName.value) {
    return t("auth.oidcLoginWithProvider", {
      provider: oidcProviderName.value,
    });
  }
  return t("auth.oidcLogin");
});
const currentLangOption = computed(() => languageOptions.find((l) => l.value === currentLanguage.value));

// Login form data
const formData = reactive<{ [key: string]: any }>({
  email: "",
  password: "",
});

// Register form data
const registerData = reactive<{ [key: string]: any }>({
  username: "",
  email: "",
  password: "",
  confirmPassword: "",
});

// Login form validation rules
const formRules = computed(() => ({
  email: [
    { required: true, message: t("auth.emailRequired"), type: "error" },
    { email: true, message: t("auth.emailInvalid"), type: "error" },
  ],
  password: [
    { required: true, message: t("auth.passwordRequired"), type: "error" },
    { min: 8, message: t("auth.passwordMinLength"), type: "error" },
    { max: 32, message: t("auth.passwordMaxLength"), type: "error" },
    {
      pattern: /[a-zA-Z]/,
      message: t("auth.passwordMustContainLetter"),
      type: "error",
    },
    {
      pattern: /\d/,
      message: t("auth.passwordMustContainNumber"),
      type: "error",
    },
  ],
}));

// Register form validation rules
const registerRules = computed(() => ({
  username: [
    { required: true, message: t("auth.usernameRequired"), type: "error" },
    { min: 2, message: t("auth.usernameMinLength"), type: "error" },
    { max: 20, message: t("auth.usernameMaxLength"), type: "error" },
    {
      pattern: /^[a-zA-Z0-9_\u4e00-\u9fa5]+$/,
      message: t("auth.usernameInvalid"),
      type: "error",
    },
  ],
  email: [
    { required: true, message: t("auth.emailRequired"), type: "error" },
    { email: true, message: t("auth.emailInvalid"), type: "error" },
  ],
  password: [
    { required: true, message: t("auth.passwordRequired"), type: "error" },
    { min: 8, message: t("auth.passwordMinLength"), type: "error" },
    { max: 32, message: t("auth.passwordMaxLength"), type: "error" },
    {
      pattern: /[a-zA-Z]/,
      message: t("auth.passwordMustContainLetter"),
      type: "error",
    },
    {
      pattern: /\d/,
      message: t("auth.passwordMustContainNumber"),
      type: "error",
    },
  ],
  confirmPassword: [
    {
      required: true,
      message: t("auth.confirmPasswordRequired"),
      type: "error",
    },
    {
      validator: (val: string) => val === registerData.password,
      message: t("auth.passwordMismatch"),
      type: "error",
    },
  ],
}));

// Toggle login/register mode
const toggleMode = () => {
  isRegisterMode.value = !isRegisterMode.value;

  Object.keys(registerData).forEach((key) => {
    (registerData as any)[key] = "";
  });
};

// Toggle language menu
const toggleLanguageMenu = () => {
  showLanguageMenu.value = !showLanguageMenu.value;
};

// Select language
const selectLanguage = (lang: string) => {
  locale.value = lang;
  localStorage.setItem("locale", lang);
  showLanguageMenu.value = false;
  MessagePlugin.success(t("language.languageSaved"));
};

// Close language menu when clicking outside
const handleClickOutside = (event: MouseEvent) => {
  const target = event.target as HTMLElement;
  if (!target.closest(".language-switch")) {
    showLanguageMenu.value = false;
  }
};

// Add click outside listener
onMounted(() => {
  document.addEventListener("click", handleClickOutside);
});

onBeforeUnmount(() => {
  document.removeEventListener("click", handleClickOutside);
});

const persistLoginResponse = async (response: any, skipRedirect = false) => {
  // Backend renamed `tenant` to `active_tenant` and added `memberships`
  // when tenant-level RBAC landed (issue #1303). The two are otherwise
  // identical — `active_tenant` is the tenant whose ID is encoded in the
  // JWT, defaulting to the user's home tenant on a fresh login.
  const activeTenant = response.active_tenant || response.tenant;
  if (response.user && response.token) {
    // user.tenant_id must be the user's HOME tenant (the immutable row
    // on the users table); useHomeTenant() and the home-badge logic both
    // assume so. The ACTIVE tenant (which can differ from home when the
    // server honoured a remembered last-active-tenant preference) is
    // expressed separately via setSelectedTenant below.
    const homeTenantIdRaw = response.user.tenant_id ?? activeTenant?.id ?? "";
    authStore.setUser(userInfoFromApi(response.user, homeTenantIdRaw));
    authStore.setToken(response.token);
    if (response.refresh_token) {
      authStore.setRefreshToken(response.refresh_token);
    }
    if (activeTenant) {
      authStore.setTenant({
        id: String(activeTenant.id) || "",
        name: activeTenant.name || "",
        owner_id: response.user.id || "",
        created_at: activeTenant.created_at || new Date().toISOString(),
        updated_at: activeTenant.updated_at || new Date().toISOString(),
      });
    } else {
      authStore.setTenant(null);
    }
    if (Array.isArray(response.memberships)) {
      authStore.setMemberships(response.memberships);
    }
    // If the backend dropped us into a non-home tenant (honoured a
    // remembered "last active tenant" preference), set the override so
    // subsequent requests carry X-Tenant-ID and the UI stays consistent.
    // Otherwise clear any stale override left in localStorage by a
    // previous session for a different account.
    const activeIdNum = Number(activeTenant?.id);
    const homeIdNum = Number(homeTenantIdRaw);
    if (Number.isFinite(activeIdNum) && Number.isFinite(homeIdNum) && activeIdNum !== homeIdNum) {
      authStore.setSelectedTenant(activeIdNum, activeTenant?.name || null);
    } else {
      authStore.setSelectedTenant(null, null);
    }
  }

  // Pull runtime capabilities (including whether ordinary users may create
  // workspaces) before entering the main UI so create actions never flash
  // briefly when the deployment is invitation-only.
  await authStore.refreshFromAuthMe();
  await nextTick();
  if (skipRedirect) return;
  router.replace(authStore.hasValidTenant ? "/platform/knowledge-bases" : "/onboarding/workspace");
};

const getBackendOIDCRedirectURI = () => `${window.location.origin}/api/v1/auth/oidc/callback`;

const loadOIDCConfig = async () => {
  try {
    const response = await getOIDCConfig();
    oidcEnabled.value = !!response.success && !!response.enabled;
    oidcProviderName.value = response.provider_display_name || "";
  } catch {
    oidcEnabled.value = false;
    oidcProviderName.value = "";
  }
};

// loadAuthConfig fetches /auth/config and caches whether self-service
// registration is allowed. Failures fall back to "enabled" so a transient
// network glitch doesn't lock new users out of an open deployment.
const loadAuthConfig = async () => {
  try {
    const response = await getAuthConfig();
    registrationEnabled.value = response.registration_mode !== "invite_only";
  } catch {
    registrationEnabled.value = true;
  }
};

const handleOIDCLogin = async () => {
  try {
    oidcLoading.value = true;
    const response = await getOIDCAuthorizationURL(getBackendOIDCRedirectURI());
    const authorizationURL = response.authorization_url;

    if (!response.success || !authorizationURL) {
      MessagePlugin.error(response.message || t("auth.oidcLoginFailed"));
      return;
    }

    // 跳转 IdP 会丢失 URL 中的 token，暂存到 sessionStorage，回调后由 App.vue 兑换。
    if (inviteToken.value) {
      sessionStorage.setItem("weknora_pending_invite_token", inviteToken.value);
    }
    window.location.href = authorizationURL;
  } catch (error: any) {
    console.error("OIDC 登录跳转失败:", error);
    MessagePlugin.error(error.message || t("auth.oidcLoginFailed"));
  } finally {
    oidcLoading.value = false;
  }
};

// 用 token 加入空间并进入应用。会话此时已有效，故即便 token 失效也照常进入（避免困在登录页）。
const acceptAndEnter = async (token: string) => {
  loading.value = true;
  try {
    const result = await authStore.acceptInvitationByTokenAndRefresh(token);
    if (result.ok) {
      MessagePlugin.success(t("inviteRegister.joined"));
    } else {
      MessagePlugin.warning(t("inviteRegister.invalidBody"));
    }
  } catch {
    MessagePlugin.warning(t("inviteRegister.invalidBody"));
  } finally {
    loading.value = false;
    await nextTick();
    router.replace("/platform/knowledge-bases");
  }
};

// Handle login
const handleLogin = async () => {
  try {
    const valid = await formRef.value?.validate();
    if (valid !== true) return;

    loading.value = true;

    const response = await login({
      email: formData.email,
      password: formData.password,
    });

    if (response.success) {
      if (inviteToken.value) {
        // 从邀请链接登录：持久化会话后兑换 token 并进入对应空间。
        await persistLoginResponse(response, true);
        await acceptAndEnter(inviteToken.value);
        return;
      }
      await persistLoginResponse(response);
      notifyLoginSuccess(response, t, tm, formatRole, roleIcon);
    } else {
      MessagePlugin.error(response.message || t("auth.loginError"));
    }
  } catch (error: any) {
    console.error("登录错误:", error);
    MessagePlugin.error(error.message || t("auth.loginErrorRetry"));
  } finally {
    loading.value = false;
  }
};

// Handle registration. Dispatches based on whether the user arrived
// with a share-link token: with token -> register-by-invite (auto-
// login on success); without -> the normal self-service register
// (drops back to the login form for the user to sign in).
const handleRegister = async () => {
  try {
    const valid = await registerFormRef.value?.validate();
    if (valid !== true) return;

    loading.value = true;

    if (inviteToken.value) {
      const response = await registerByInvite({
        token: inviteToken.value,
        username: registerData.username,
        email: registerData.email,
        password: registerData.password,
      });
      if (!response.success) {
        MessagePlugin.error(response.message || t("auth.registerFailed"));
        return;
      }
      MessagePlugin.success(t("auth.registerSuccess"));
      // register-by-invite returns the same shape as login (token +
      // active_tenant + memberships), so reuse the login persistence
      // path — same store writes, same redirect target.
      await persistLoginResponse(response);
      return;
    }

    const response = await register({
      username: registerData.username,
      email: registerData.email,
      password: registerData.password,
    });

    if (response.success) {
      MessagePlugin.success(t("auth.registerSuccess"));

      // Switch to login mode and fill in email
      isRegisterMode.value = false;
      formData.email = registerData.email;

      // Clear register form
      Object.keys(registerData).forEach((key) => {
        (registerData as any)[key] = "";
      });
    } else {
      MessagePlugin.error(response.message || t("auth.registerFailed"));
    }
  } catch (error: any) {
    console.error("注册错误:", error);
    MessagePlugin.error(error.message || t("auth.registerError"));
  } finally {
    loading.value = false;
  }
};

// Check if already logged in; for lite edition, attempt transparent auto-setup
onMounted(async () => {
  // Share-link landing: ?token=xxx switches the form into invite-
  // register mode before any other auto-flow (logged-in redirect /
  // auto-setup / OIDC) gets a chance to redirect. Resolution failure
  // surfaces inline; the user can still log in normally if they
  // already have an account. We check this BEFORE the isLoggedIn
  // redirect so an existing session doesn't bounce the user to
  // /platform (and possibly back to /login if the session is stale),
  // dropping the invite token along the way.
  const tokenFromQuery = String(route.query.token || "").trim();
  if (tokenFromQuery) {
    inviteToken.value = tokenFromQuery;
    inviteLookupLoading.value = true;
    // 1. 先校验 token：无效/过期则停在登录页报错，不进注册模式。
    try {
      const resp = await getInvitationByToken(tokenFromQuery);
      if (resp.success && resp.data) {
        inviteLookup.value = resp.data;
      } else {
        inviteLookupError.value = resp.message || t("inviteRegister.invalidBody");
        loadOIDCConfig();
        loadAuthConfig();
        return;
      }
    } catch {
      inviteLookupError.value = t("inviteRegister.invalidBody");
      loadOIDCConfig();
      loadAuthConfig();
      return;
    } finally {
      inviteLookupLoading.value = false;
    }

    // 2. 已登录则直接兑换 token 进入空间（两种模式通用）。
    if (authStore.isLoggedIn && (await authStore.refreshFromAuthMe())) {
      await acceptAndEnter(tokenFromQuery);
      return;
    }

    // 3. 未登录：按注册模式决定界面。invite_only 停在登录页、登录后再兑换；self_serve 保持注册流程。
    const cfg = await getAuthConfig();
    const inviteOnly = cfg.registration_mode === "invite_only";
    registrationEnabled.value = !inviteOnly;
    isRegisterMode.value = !inviteOnly;
    loadOIDCConfig();
    return;
  }

  if (authStore.isLoggedIn) {
    router.replace("/platform/knowledge-bases");
    return;
  }

  const AUTO_SETUP_FAILED_KEY = "weknora_auto_setup_failed";
  if (localStorage.getItem(AUTO_SETUP_FAILED_KEY) !== "true") {
    try {
      const response = await autoSetup();
      if (response.success) {
        authStore.setLiteMode(true);
        await persistLoginResponse(response);
        return;
      } else {
        localStorage.setItem(AUTO_SETUP_FAILED_KEY, "true");
      }
    } catch {
      localStorage.setItem(AUTO_SETUP_FAILED_KEY, "true");
    }
  }

  loadOIDCConfig();
  loadAuthConfig();
});
</script>

<style lang="less" scoped>
.login-layout {
  width: 100%;
  min-height: 100%;
  // display: flex;
  // flex-direction: column;
  // justify-content: flex-end;
  // align-items: center; /* 水平方向居中 */
  overflow: hidden;

  color: #fff;
  background:
    radial-gradient(900px 620px at 12% 8%, rgba(52, 211, 153, 0.16), transparent 62%), radial-gradient(760px 560px at 88% 92%, rgba(16, 185, 129, 0.12), transparent 60%),
    linear-gradient(135deg, #052e22 0%, #0a4a36 52%, #0e6b4f 100%);
  min-height: 99vh;
  overflow: hidden !important;
  -webkit-font-smoothing: antialiased;
  display: flex;
  flex-direction: column;
}
/* ============ 背景装饰：网格 + 数据星座 ============ */
.bg-grid {
  position: fixed;
  inset: 0;
  pointer-events: none;
  background: repeating-linear-gradient(0deg, rgba(255, 255, 255, 0.028) 0 1px, transparent 1px 72px), repeating-linear-gradient(90deg, rgba(255, 255, 255, 0.028) 0 1px, transparent 1px 72px);
  mask-image: radial-gradient(1200px 800px at 50% 40%, #000 30%, transparent 100%);
}
/* 网格 */
.bg-net {
  position: fixed;
  inset: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  opacity: 0.9;
}
/*连线 */
.net-dash {
  stroke-dasharray: 5 9;
  animation: flow 26s linear infinite;
}
@keyframes flow {
  to {
    stroke-dashoffset: -560;
  }
}
.float-a {
  animation: floatY 9s ease-in-out infinite;
}
.float-b {
  animation: floatY 12s ease-in-out infinite reverse;
}
@keyframes floatY {
  0%,
  100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-14px);
  }
}
/*线的动画 */
.glow {
  position: fixed;
  border-radius: 50%;
  filter: blur(90px);
  pointer-events: none;
  animation: drift 18s ease-in-out infinite alternate;
}
.glow-1 {
  //width: 420px;
  //height: 420px;
  left: -120px;
  top: -120px;
  background: rgba(16, 185, 129, 0.2);
}
.glow-2 {
  //width: 360px;
  //height: 360px;
  right: -100px;
  bottom: -120px;
  background: rgba(110, 231, 183, 0.12);
}
@keyframes drift {
  to {
    transform: translate(40px, 26px);
  }
}
/* 漂浮信息玻璃片 */
.float-chip {
  position: absolute;
  display: flex;
  align-items: center;
  gap: 9px;
  padding: 11px 16px;
  border-radius: 12px;
  // background: rgba(10, 40, 30, 0.55);
  border: 1px solid rgba(110, 231, 183, 0.3);
  // backdrop-filter: blur(10px);
  font-size: 12.5px;
  color: rgba(224, 242, 237, 0.9);
  box-shadow: 0 14px 34px rgba(2, 20, 14, 0.35);
}
.float-chip .fc-ic {
  width: 26px;
  height: 26px;
  border-radius: 8px;
  display: grid;
  place-items: center;
  // background: rgba(52, 211, 153, 0.18);
  color: #6ee7b7;
  flex: none;
}
.float-chip b {
  color: #a7f3d0;
  font-weight: 600;
}
.fc-1 {
  top: 14%;
  left: 56%;
  animation: floatY 8s ease-in-out infinite;
}
.fc-2 {
  bottom: 12%;
  left: 4%;
  animation: floatY 11s ease-in-out 1.2s infinite;
}
/* ============ 页面框架 page ============ */
/*头部小云智问的标题 */
.topbar {
  display: flex;
  flex: none; // 保持原样的大小
  justify-content: space-between;
  padding: 0.7rem;
}
// 小云智问标题
.brand {
  display: flex;
  align-items: center;
  gap: 12px;
  color: #fff;
}
// 政务内网
.net-chip {
  display: flex;
  align-items: center;
  gap: 7px;
  padding: 8px 14px;
  border-radius: 999px;
  background: rgba(255, 255, 255, 0.07);
  border: 1px solid rgba(110, 231, 183, 0.28);
  font-size: 12.5px;
  color: #a7f3d0;
  // backdrop-filter: blur(6px);
}
// 左侧的圆角
.eyebrow {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 8px 15px;
  border-radius: 999px;
  background: rgba(110, 231, 183, 0.1);
  border: 1px solid rgba(110, 231, 183, 0.35);
  color: #6ee7b7;
  font-size: 13px;
  font-weight: 500;
  letter-spacing: 1px;
  animation: rise 0.7s 0.05s cubic-bezier(0.2, 0.7, 0.2, 1) both;
}
.eyebrow::before {
  content: "";
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: #34d399;
  box-shadow: 0 0 10px #34d399;
}

.brand-mark {
  width: 36px;
  height: 36px;
  border-radius: 10px;
  display: grid;
  place-items: center;
  flex: none;
  background: linear-gradient(135deg, #34d399, #059669);
  box-shadow: 0 6px 18px rgba(16, 185, 129, 0.45);
}

.brand-name {
  font-size: 18px;
  font-weight: 700;
  letter-spacing: 0.5px;
}

.brand-div {
  width: 1px;
  height: 16px;
  background: rgba(255, 255, 255, 0.28);
}

.brand-sub {
  font-size: 12.5px;
  color: rgba(224, 242, 237, 0.62);
  letter-spacing: 1px;
}

// 主要的内容区域
.main-container {
  display: flex;
  flex: 1; // 占满剩余的空间
  padding: 0.5rem;
  // justify-content: space-between;
  justify-content: space-around;
  align-items: center;
}
.hero {
  flex: 1.15;
  max-width: 660px;
  min-width: 0;
  height: 50vh;
}

.hero h1 {
  margin: 22px 0 18px;
  font-size: clamp(30px, 3.4vw, 44px);
  font-weight: 700;
  line-height: 1.32;
  letter-spacing: 0.5px;
  animation: rise 0.7s 0.15s cubic-bezier(0.2, 0.7, 0.2, 1) both;
}
.hero h1 .grad {
  background: linear-gradient(92deg, #6ee7b7 10%, #d1fae5 90%);
  -webkit-background-clip: text;
  background-clip: text;
  color: transparent;
}
.hero h1 .dot {
  color: #34d399;
  margin: 0 10px;
  font-weight: 400;
}
.hero .sub {
  max-width: 560px;
  font-size: 15.5px;
  line-height: 1.95;
  color: rgba(224, 242, 237, 0.8);
  animation: rise 0.7s 0.25s cubic-bezier(0.2, 0.7, 0.2, 1) both;
}
.hero .sub b {
  color: #a7f3d0;
  font-weight: 600;
}

/* 四大能力卡片 */
.caps {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 12px;
  margin-top: 30px;
}
.cap {
  display: flex;
  gap: 13px;
  padding: 16px 17px;
  border-radius: 14px;
  background: rgba(255, 255, 255, 0.055);
  border: 1px solid rgba(255, 255, 255, 0.12);
  // backdrop-filter: blur(8px);
  transition: 0.28s;
  animation: rise 0.7s cubic-bezier(0.2, 0.7, 0.2, 1) both;
}
.cap:nth-child(1) {
  animation-delay: 0.35s;
}
.cap:nth-child(2) {
  animation-delay: 0.43s;
}
.cap:nth-child(3) {
  animation-delay: 0.51s;
}
.cap:nth-child(4) {
  animation-delay: 0.59s;
}
.cap:hover {
  background: rgba(255, 255, 255, 0.1);
  border-color: rgba(110, 231, 183, 0.4);
  transform: translateY(-3px);
}
.cap-ic {
  width: 38px;
  height: 38px;
  border-radius: 10px;
  flex: none;
  display: grid;
  place-items: center;
  background: rgba(52, 211, 153, 0.14);
  border: 1px solid rgba(110, 231, 183, 0.3);
  color: #6ee7b7;
}
.cap h3 {
  font-size: 14.5px;
  font-weight: 600;
  letter-spacing: 0.3px;
  margin-bottom: 5px;
}
.cap p {
  font-size: 12.5px;
  line-height: 1.75;
  color: rgba(209, 250, 229, 0.62);
}

/* 数据条 */
.stats {
  display: flex;
  margin-top: 32px;
  padding-top: 24px;
  border-top: 1px solid rgba(255, 255, 255, 0.12);
  animation: rise 0.7s 0.68s cubic-bezier(0.2, 0.7, 0.2, 1) both;
}
.stat {
  flex: 1;
  min-width: 0;
}
.stat + .stat {
  border-left: 1px solid rgba(255, 255, 255, 0.1);
  padding-left: 22px;
  margin-left: 22px;
}
.stat .num {
  font-size: 27px;
  font-weight: 700;
  color: #a7f3d0;
  font-variant-numeric: tabular-nums;
  letter-spacing: 0.5px;
}
.stat .num small {
  font-size: 15px;
  font-weight: 600;
  margin-left: 2px;
}
.stat .lbl {
  font-size: 12px;
  color: rgba(197, 231, 215, 0.6);
  margin-top: 5px;
  letter-spacing: 0.5px;
  white-space: nowrap;
}

/* 漂浮信息玻璃片 */
.float-chip {
  position: absolute;
  display: flex;
  align-items: center;
  gap: 9px;
  padding: 11px 16px;
  border-radius: 12px;
  // background: rgba(10, 40, 30, 0.55);
  border: 1px solid rgba(110, 231, 183, 0.3);
  // backdrop-filter: blur(10px);
  font-size: 12.5px;
  color: rgba(224, 242, 237, 0.9);
  box-shadow: 0 14px 34px rgba(2, 20, 14, 0.35);
}
.float-chip .fc-ic {
  width: 26px;
  height: 26px;
  border-radius: 8px;
  display: grid;
  place-items: center;
  background: rgba(52, 211, 153, 0.18);
  color: #6ee7b7;
  flex: none;
}
.float-chip b {
  color: #a7f3d0;
  font-weight: 600;
}
.fc-1 {
  top: 14%;
  left: 56%;
  animation: floatY 8s ease-in-out infinite;
  opacity: 10%;
}
.fc-2 {
  bottom: 12%;
  left: 4%;
  animation: floatY 11s ease-in-out 1.2s infinite;
  opacity: 10%;
}

/* Right Form Section */
.form-section {
  flex: 0 0 48%;
  display: flex;
  align-items: flex-end;
  justify-content: center;
  padding: 40px 50px 100px 30px;
  box-sizing: border-box;
  position: relative;
}

.form-panel {
  width: 100%;
  max-width: 480px;
  margin-bottom: 60px;
  position: relative;
  z-index: 2;
}

.form-card {
  background: rgba(255, 255, 255, 0.97);
  border-radius: 16px;
  padding: 40px;
  box-shadow: 0 10px 40px rgba(0, 0, 0, 0.15);
  box-sizing: border-box;
  border: none;
  width: 100%;
}

.form-header {
  text-align: center;
  margin-bottom: 32px;
}

.form-title {
  font-size: 24px;
  font-weight: 600;
  color: var(--td-text-color-primary);
  margin: 0 0 6px 0;
  font-family: var(--app-font-family);
}

.form-welcome {
  font-size: 13px;
  color: var(--td-text-color-secondary);
  margin: 0;
  font-family: var(--app-font-family);
}

.form-hint {
  margin: 10px 0 0;
  padding: 8px 12px;
  border-radius: 8px;
  background: var(--td-success-color-light, rgba(7, 192, 95, 0.08));
  color: var(--td-brand-color-active);
  font-size: 12.5px;
  line-height: 1.5;
  font-family: var(--app-font-family);
}

.form-footer {
  text-align: center;
  font-size: 14px;
  color: var(--td-text-color-secondary);
  font-family: var(--app-font-family);
  margin-top: 16px;
  padding-bottom: 16px;
  border-bottom: 1px solid var(--td-component-stroke);

  .link-button {
    color: var(--td-brand-color);
    text-decoration: none;
    margin-left: 4px;
    font-weight: 500;
    transition: all 0.2s;

    &:hover {
      color: var(--td-brand-color);
      text-decoration: underline;
    }
  }
}

.login-form-footer {
  border-bottom: none;
  padding-bottom: 8px;
  margin-top: 12px;
}

.login-features {
  margin-top: 20px;
  padding: 0;

  .feature-item {
    display: flex;
    align-items: center;
    margin-bottom: 12px;
    font-size: 13px;
    color: var(--td-text-color-secondary);
    font-family: var(--app-font-family);

    &:last-child {
      margin-bottom: 0;
    }

    .feature-icon {
      width: 20px;
      height: 20px;
      border-radius: 50%;
      background: var(--td-success-color-light);
      color: var(--td-brand-color-active);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 12px;
      font-weight: 700;
      margin-right: 10px;
      flex-shrink: 0;
    }

    .feature-text {
      line-height: 1.4;
    }
  }
}

/* Responsive Design */
@media (max-width: 1024px) {
  .knowledge-node:nth-of-type(n + 13) {
    display: none;
  }

  .connection-line:nth-of-type(n + 13) {
    display: none;
  }

  .showcase-subtitle {
    font-size: 18px;
  }

  .header-logo {
    top: 26px;
    left: 40px;

    .logo-image {
      width: 100px;
    }
  }

  .header-links {
    top: 22px;
    right: 22px;
    gap: 8px;

    .link-text {
      display: none;
    }

    .header-link {
      padding: 10px;
      gap: 0;
    }
  }
}

@media (max-width: 768px) {
  .login-layout {
    flex-direction: column;
  }

  .knowledge-node:nth-of-type(n + 9) {
    display: none;
  }

  .connection-line:nth-of-type(n + 9) {
    display: none;
  }

  .showcase-section {
    flex: 0 0 auto;
    min-height: 50vh;
    padding: 40px 24px;
  }

  .showcase-content {
    max-width: 100%;
  }

  .header-logo {
    top: 22px;
    left: 30px;

    .logo-image {
      width: 80px;
    }
  }

  .showcase-subtitle {
    font-size: 16px;
    margin-bottom: 24px;
  }

  .feature-tags {
    margin-bottom: 24px;
  }

  .carousel-container {
    margin-top: 24px;
  }

  .form-section {
    flex: 0 0 auto;
    padding: 24px;
  }

  .header-links {
    top: 18px;
    right: 18px;
    gap: 8px;

    .link-text {
      display: inline;
    }

    .header-link {
      padding: 8px 12px;
      font-size: 12px;
    }
  }

  .form-card {
    padding: 32px 24px;
  }

  .form-title {
    font-size: 22px;
  }
}

@media (max-width: 480px) {
  .animated-bg {
    display: none;
  }

  .showcase-section {
    padding: 32px 20px;
  }

  .header-logo {
    top: 18px;
    left: 20px;

    .logo-image {
      width: 70px;
    }
  }

  .showcase-subtitle {
    font-size: 14px;
  }

  .tag {
    font-size: 12px;
    padding: 6px 16px;
  }

  .form-section {
    padding: 20px;
  }

  .header-links {
    top: 14px;
    right: 14px;
    gap: 6px;
    flex-wrap: wrap;

    .header-link {
      padding: 7px 10px;
      font-size: 11px;
    }
  }

  .form-card {
    padding: 28px 20px;
  }

  .form-header {
    margin-bottom: 24px;
  }
}

@media (prefers-reduced-motion: reduce) {
  .knowledge-node,
  .connection-line {
    animation: none !important;
    transition: none !important;
  }

  .animated-bg {
    display: none;
  }
}
</style>

<style lang="less">
html[theme-mode="dark"] {
  .login-layout {
    background: linear-gradient(225deg, #011a14 0%, #032e22 15%, #043a2c 25%, #05503d 38%, #046647 50%, #038a56 65%, #049b60 78%, #06a06a 90%, #07b074 100%);
  }

  .knowledge-node {
    background: rgba(255, 255, 255, 0.1);
    border-color: rgba(255, 255, 255, 0.2);
    box-shadow: 0 0 8px rgba(255, 255, 255, 0.15);
  }

  .connection-line {
    stroke: rgba(255, 255, 255, 0.25);
  }

  .header-logo .logo-image {
    filter: invert(1) hue-rotate(180deg) brightness(1.1);
  }

  .header-link {
    background: rgba(255, 255, 255, 0.12);
    border-color: rgba(255, 255, 255, 0.15);

    &:hover {
      background: rgba(255, 255, 255, 0.2);
    }
  }

  .language-switch button {
    background: rgba(255, 255, 255, 0.12);
    border-color: rgba(255, 255, 255, 0.15);

    &:hover {
      background: rgba(255, 255, 255, 0.2);
    }
  }

  .language-dropdown {
    background: rgba(36, 36, 36, 0.97) !important;
    border-color: var(--td-component-stroke) !important;
    box-shadow: 0 4px 16px rgba(0, 0, 0, 0.4) !important;
  }

  .tag {
    background: rgba(255, 255, 255, 0.12);
  }

  .form-card {
    background: rgba(36, 36, 36, 0.97) !important;
    box-shadow: 0 10px 40px rgba(0, 0, 0, 0.4) !important;
  }

  .register-cta__divider span {
    background: rgba(36, 36, 36, 0.97);
  }

  .form-content .t-input {
    background: var(--td-bg-color-page) !important;
    border-color: rgba(255, 255, 255, 0.1) !important;

    &:hover {
      border-color: var(--td-brand-color) !important;
    }

    &:focus-within {
      border-color: var(--td-brand-color) !important;
    }
  }

  .screenshot-swiper .swiper-pagination-bullet-active {
    background: rgba(255, 255, 255, 0.9) !important;
  }

  .login-features .feature-icon {
    background: rgba(6, 176, 77, 0.15);
  }
}
</style>
