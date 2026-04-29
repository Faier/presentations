<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <img src="/solo.png" alt="SOP" class="company-logo" />
    <div class="cta-container">
      <div class="cta-glow glow-1"></div>
      <div class="cta-glow glow-2"></div>
      <div class="text-center relative z-10">
        <h2 class="text-5xl font-black tracking-tight text-transparent bg-clip-text bg-gradient-to-r from-indigo-400 via-purple-400 to-emerald-400">
          感谢关注
        </h2>
        <p class="mt-6 text-xl text-slate-600">Auto-Generate-Rule 医疗规则自动生成</p>

        <!-- Stats -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mt-10 max-w-3xl mx-auto">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-4xl font-black text-transparent bg-clip-text bg-gradient-to-r from-indigo-500 to-emerald-400">80%</div>
            <div class="mt-2 text-sm text-slate-600">CDSS 配置需求已自动化</div>
          </div>
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-4xl font-black text-transparent bg-clip-text bg-gradient-to-r from-amber-500 to-rose-400">20%</div>
            <div class="mt-2 text-sm text-slate-600">定制需求按原方式处理</div>
          </div>
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-4xl font-black text-transparent bg-clip-text bg-gradient-to-r from-emerald-400 to-sky-400">&#8734;</div>
            <div class="mt-2 text-sm text-slate-600">病历质控 / 医保稽核 / 更多</div>
          </div>
        </div>

        <div class="mt-12 flex flex-wrap items-center justify-center gap-3">
          <span class="px-4 py-2 rounded-full bg-gradient-to-r from-indigo-500/10 to-emerald-400/10 border border-indigo-200/30 text-sm font-semibold text-indigo-600">CDSS</span>
          <span class="px-4 py-2 rounded-full bg-gradient-to-r from-indigo-500/10 to-emerald-400/10 border border-indigo-200/30 text-sm font-semibold text-purple-600">Claude Code</span>
          <span class="px-4 py-2 rounded-full bg-gradient-to-r from-indigo-500/10 to-emerald-400/10 border border-indigo-200/30 text-sm font-semibold text-amber-600">医疗 AI</span>
        </div>
        </div>
    </div>
  </section>
</template>

<style scoped>
.slide-shell {
  display: flex;
  height: 100%;
  width: 100%;
  align-items: center;
  justify-content: center;
  padding: clamp(3rem, 8vw, 7rem);
  background: radial-gradient(120% 140% at 50% 50%, rgba(99, 102, 241, 0.1), transparent 60%),
    #f8fafc;
  position: relative;
}

.company-logo {
  position: absolute;
  top: 1.5rem;
  left: 2rem;
  height: 48px;
  width: auto;
  z-index: 20;
  opacity: 0.85;
}

.cta-container {
  position: relative;
  text-align: center;
}

.cta-glow {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  pointer-events: none;
}

.glow-1 {
  width: 400px;
  height: 400px;
  top: -150px;
  left: -100px;
  background: radial-gradient(circle, rgba(99, 102, 241, 0.25), transparent 70%);
}

.glow-2 {
  width: 350px;
  height: 350px;
  bottom: -100px;
  right: -100px;
  background: radial-gradient(circle, rgba(16, 185, 129, 0.2), transparent 70%);
}
</style>
