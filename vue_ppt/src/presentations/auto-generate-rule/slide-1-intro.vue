<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <img src="/solo.png" alt="SOP" class="company-logo" />
    <div class="hero-container">
      <div class="hero-glow glow-1"></div>
      <div class="hero-glow glow-2"></div>
      <div class="hero-content">
        <h1 class="hero-title">
          <span class="title-gradient">Auto-Generate-Rule</span>
          <span class="hero-subtitle">基于CLaude Code SKill生成的医疗规则</span>
        </h1>
        <div class="feature-row">
          <div class="feature-badge">&#x1F4DD; 自然语言输入</div>
          <span class="feature-sep">+</span>
          <div class="feature-badge">&#x1F91D; 约定 &gt; 配置</div>
          <span class="feature-sep">+</span>
          <div class="feature-badge">&#x1F4E6; 批量生成</div>
        </div>
        <div class="pain-row">
          <div class="pain-item">
            <span class="pain-marker">&#x26A0;</span>
            入手门槛高
          </div>
          <div class="pain-item">
            <span class="pain-marker">&#x26A0;</span>
            配置灵活却难以理解
          </div>
          <div class="pain-item">
            <span class="pain-marker">&#x26A0;</span>
            规则配置需求多，耗时耗力
          </div>
        </div>
        <div class="hero-badges">
          <span class="badge">自然语言输入</span>
          <span class="badge">AI分析</span>
          <span class="badge">一键确认写入</span>
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

.hero-container {
  position: relative;
  max-width: min(92vw, 1000px);
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
  gap: 0.8rem;
}

.title-gradient {
  font-size: clamp(3rem, 8vw, 5.5rem);
  font-weight: 900;
  letter-spacing: -0.04em;
  line-height: 1.1;
  background: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #10b981 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-subtitle {
  font-size: clamp(1.8rem, 4vw, 2.8rem);
  font-weight: 400;
  color: #64748b;
  letter-spacing: -0.02em;
}

.feature-row {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  gap: 0.6rem;
  margin-top: 1.5rem;
}

.feature-badge {
  padding: 0.4rem 1rem;
  border-radius: 9999px;
  background: linear-gradient(135deg, rgba(99, 102, 241, 0.08), rgba(16, 185, 129, 0.06));
  border: 1px solid rgba(99, 102, 241, 0.15);
  font-size: 0.9rem;
  font-weight: 600;
  color: #475569;
  white-space: nowrap;
}

.feature-sep {
  font-size: 0.85rem;
  color: #cbd5e1;
  font-weight: 500;
}

.pain-row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1.5rem;
  margin-top: 1rem;
}

.pain-item {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  font-size: 0.95rem;
  color: #ef4444;
  font-weight: 600;
}

.pain-marker {
  font-size: 1.1rem;
}

.hero-badges {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 0.75rem;
  margin-top: 2rem;
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
