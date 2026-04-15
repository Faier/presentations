<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">其他热门项目</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="flex items-center gap-3 mb-4">
            <div class="px-3 py-1 bg-emerald-100 text-emerald-700 text-sm font-bold rounded-full">1,035 ⭐</div>
            <div class="text-xl font-bold text-slate-800">Harness Engineering</div>
          </div>
          <p class="text-slate-600 mb-4">
            ZhangHanDong 开源的项目，从 Claude Code 源码角度深入探讨 Harness 工程化实践。
          </p>
          <div class="flex flex-wrap gap-2">
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">源码分析</span>
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">AI Coding</span>
          </div>
        </div>
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="flex items-center gap-3 mb-4">
            <div class="px-3 py-1 bg-indigo-100 text-indigo-700 text-sm font-bold rounded-full">532 ⭐</div>
            <div class="text-xl font-bold text-slate-800">Claude Code Harness</div>
          </div>
          <p class="text-slate-600 mb-4">
            Chachamaru127 的专用开发 Harness，通过自主 Plan→Work→Review 循环实现高质量开发。
          </p>
          <div class="flex flex-wrap gap-2">
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">自动化</span>
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">Review Cycle</span>
          </div>
        </div>
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="flex items-center gap-3 mb-4">
            <div class="px-3 py-1 bg-purple-100 text-purple-700 text-sm font-bold rounded-full">-</div>
            <div class="text-xl font-bold text-slate-800">EveryThing Claude Code</div>
          </div>
          <p class="text-slate-600 mb-4">
            affaan-m 的性能优化系统，涵盖 Skills、Instincts、Memory、Security 和研究优先的开发方法。
          </p>
          <div class="flex flex-wrap gap-2">
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">性能优化</span>
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">Production</span>
          </div>
        </div>
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="flex items-center gap-3 mb-4">
            <div class="px-3 py-1 bg-amber-100 text-amber-700 text-sm font-bold rounded-full">-</div>
            <div class="text-xl font-bold text-slate-800">Oh-My-OpenAgent</div>
          </div>
          <p class="text-slate-600 mb-4">
            code-yeongyu 开发的最佳 agent harness，前身是 oh-my-opencode，提供简洁优雅的 agent 框架。
          </p>
          <div class="flex flex-wrap gap-2">
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">框架</span>
            <span class="px-3 py-1 bg-slate-100 rounded-full text-xs">轻量</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>