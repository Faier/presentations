<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="hero-container">
      <div class="hero-glow glow-1"></div>
      <div class="hero-glow glow-2"></div>
      <div class="hero-content">
        <h1 class="hero-title">
          <span class="title-gradient">Claude Agent Harness</span>
          <span class="hero-subtitle">深度解析</span>
        </h1>
        <p class="hero-tagline">用 AI + 代码解决一切问题</p>
        <div class="hero-badges">
          <span class="badge">Skills</span>
          <span class="badge">Memory</span>
          <span class="badge">Security</span>
          <span class="badge">Agent Loop</span>
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
  background: radial-gradient(120% 140% at 85% 10%, rgba(99, 102, 241, 0.15), transparent 55%),
    radial-gradient(90% 120% at 10% 90%, rgba(16, 185, 129, 0.1), transparent 60%),
    #f8fafc;
}

.hero-container {
  position: relative;
  max-width: min(92vw, 1200px);
  text-align: center;
}

.hero-glow {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  pointer-events: none;
}

.glow-1 {
  width: 400px;
  height: 400px;
  top: -100px;
  right: -100px;
  background: radial-gradient(circle, rgba(99, 102, 241, 0.3), transparent 70%);
}

.glow-2 {
  width: 300px;
  height: 300px;
  bottom: -50px;
  left: -50px;
  background: radial-gradient(circle, rgba(16, 185, 129, 0.25), transparent 70%);
}

.hero-content {
  position: relative;
  z-index: 1;
}

.hero-title {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.title-gradient {
  font-size: clamp(3rem, 8vw, 6rem);
  font-weight: 900;
  letter-spacing: -0.04em;
  line-height: 1.1;
  background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #10b981 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-subtitle {
  font-size: clamp(2rem, 5vw, 3.5rem);
  font-weight: 700;
  color: #1e293b;
  letter-spacing: -0.02em;
}

.hero-tagline {
  margin-top: 2rem;
  font-size: clamp(1.1rem, 2vw, 1.5rem);
  color: #64748b;
  font-weight: 500;
}

.hero-badges {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 0.75rem;
  margin-top: 2.5rem;
}

.badge {
  padding: 0.5rem 1.25rem;
  border-radius: 9999px;
  background: linear-gradient(135deg, rgba(99, 102, 241, 0.1), rgba(16, 185, 129, 0.1));
  border: 1px solid rgba(99, 102, 241, 0.2);
  font-size: 0.9rem;
  font-weight: 600;
  color: #6366f1;
}
</style>