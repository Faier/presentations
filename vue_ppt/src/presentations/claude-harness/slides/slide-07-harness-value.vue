<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Harness 的核心价值</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="p-8 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl text-center">
          <div class="text-5xl mb-4">🎯</div>
          <div class="text-2xl font-bold text-indigo-600 mb-3">可预测性</div>
          <p class="text-slate-600">通过结构化的执行循环和约束机制，让 AI 输出更加稳定可靠</p>
        </div>
        <div class="p-8 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl text-center">
          <div class="text-5xl mb-4">🔄</div>
          <div class="text-2xl font-bold text-emerald-600 mb-3">可组合性</div>
          <p class="text-slate-600">Skills 和 Tools 可以像乐高积木一样自由组合，快速构建复杂能力</p>
        </div>
        <div class="p-8 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl text-center">
          <div class="text-5xl mb-4">🛡️</div>
          <div class="text-2xl font-bold text-amber-600 mb-3">安全性</div>
          <p class="text-slate-600">细粒度的权限控制和审计日志，确保 AI 行为在可控范围内</p>
        </div>
        <div class="p-8 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl text-center">
          <div class="text-5xl mb-4">🔧</div>
          <div class="text-2xl font-bold text-purple-600 mb-3">可扩展性</div>
          <p class="text-slate-600">开放的架构设计，支持自定义 Skills、Tools 和 Memory 后端</p>
        </div>
      </div>
    </div>
  </section>
</template>