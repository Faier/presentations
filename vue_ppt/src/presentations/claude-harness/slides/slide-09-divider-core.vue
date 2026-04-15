<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="divider-container">
      <div class="divider-glow"></div>
      <div class="text-center">
        <div class="text-sm font-semibold text-emerald-500 tracking-widest uppercase mb-4">第三章</div>
        <h2 class="text-6xl font-black tracking-tight text-transparent bg-clip-text bg-gradient-to-r from-indigo-400 via-purple-400 to-emerald-400">
          核心组件
        </h2>
        <p class="mt-6 text-xl text-slate-600">构建强大 Agent 的基石</p>
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
  background: radial-gradient(ellipse 80% 50% at 50% 50%, rgba(16, 185, 129, 0.12), transparent),
    #f8fafc;
}

.divider-container {
  position: relative;
  text-align: center;
}

.divider-glow {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 600px;
  height: 300px;
  background: radial-gradient(ellipse, rgba(16, 185, 129, 0.15), transparent 70%);
  filter: blur(60px);
  pointer-events: none;
}
</style>