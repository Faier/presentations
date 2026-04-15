<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="cta-container">
      <div class="cta-glow glow-1"></div>
      <div class="cta-glow glow-2"></div>
      <div class="text-center relative z-10">
        <h2 class="text-5xl font-black tracking-tight text-transparent bg-clip-text bg-gradient-to-r from-indigo-400 via-purple-400 to-emerald-400">
          如果有用，点赞 + 关注
        </h2>
        <p class="mt-6 text-xl text-slate-600">这只是 AI Agent Harness 系列的开始</p>
        <div class="mt-10 flex items-center justify-center gap-6">
          <div class="px-8 py-4 rounded-full bg-gradient-to-r from-indigo-500 to-purple-500 text-white font-bold shadow-xl hover:shadow-2xl transition-all cursor-pointer">
            ⭐ Star 本项目
          </div>
          <div class="px-8 py-4 rounded-full bg-white/60 border border-white/40 backdrop-blur-md text-slate-700 font-bold shadow-lg hover:shadow-xl transition-all cursor-pointer">
            关注作者
          </div>
        </div>
        <div class="mt-12 text-sm text-slate-500">
          Claude Agent Harness 深度解析 | 基于 presentations_by_ai 构建
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