<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <img src="/solo.png" alt="SOP" class="company-logo" />
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 text-center mb-8">怎么创建一个 Skill</h2>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Left: Steps -->
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="flex items-center gap-3 mb-4">
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-gradient-to-br from-indigo-500 to-purple-500 text-white font-extrabold text-lg flex-shrink-0">1</span>
              <span class="text-xl font-bold text-indigo-600">克隆官方仓库</span>
            </div>
            <div class="bg-slate-900 text-emerald-400 font-mono text-sm px-4 py-3 rounded-xl overflow-x-auto">
              git clone https://github.com/anthropics/skills
            </div>
          </div>

          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="flex items-center gap-3 mb-4">
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-gradient-to-br from-indigo-500 to-purple-500 text-white font-extrabold text-lg flex-shrink-0">2</span>
              <span class="text-xl font-bold text-indigo-600">找到 skill-creator</span>
            </div>
            <div class="bg-slate-900 text-sky-300 font-mono text-sm px-4 py-3 rounded-xl overflow-x-auto">
              skills/skill-creator/
            </div>
          </div>

          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="flex items-center gap-3 mb-4">
              <span class="flex items-center justify-center w-10 h-10 rounded-full bg-gradient-to-br from-indigo-500 to-purple-500 text-white font-extrabold text-lg flex-shrink-0">3</span>
              <span class="text-xl font-bold text-indigo-600">复制到技能目录</span>
            </div>
            <div class="bg-slate-900 text-amber-300 font-mono text-sm px-4 py-3 rounded-xl overflow-x-auto">
              C:\Users\jiang\.claude\skills\
            </div>
          </div>
        </div>

        <!-- Right: Result -->
        <div class="flex items-center justify-center">
          <div class="p-8 bg-gradient-to-br from-indigo-500/10 to-emerald-400/10 border border-indigo-200/30 rounded-3xl text-center w-full shadow-xl">
            <div class="text-5xl mb-4">&#x2728;</div>
            <div class="text-2xl font-extrabold text-slate-700 mb-1">用 skill-creator</div>
            <div class="text-base text-slate-500 mb-6">创建你自己的技能</div>
            <div class="space-y-3 text-left max-w-[260px] mx-auto">
              <div class="flex items-center gap-2 text-slate-600 font-medium">
                <span class="text-emerald-500 font-bold text-lg">&#10003;</span> 定义触发词
              </div>
              <div class="flex items-center gap-2 text-slate-600 font-medium">
                <span class="text-emerald-500 font-bold text-lg">&#10003;</span> 编写工作流
              </div>
              <div class="flex items-center gap-2 text-slate-600 font-medium">
                <span class="text-emerald-500 font-bold text-lg">&#10003;</span> 定义输出模板
              </div>
            </div>
          </div>
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
  background: radial-gradient(120% 140% at 10% 90%, rgba(16, 185, 129, 0.1), transparent 60%),
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
</style>
