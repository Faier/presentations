<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Claude 模型家族</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="p-6 bg-gradient-to-br from-slate-800 to-slate-900 text-white rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-slate-400 mb-2">Haiku 3</div>
          <div class="text-3xl font-black mb-4">轻量快速</div>
          <ul class="space-y-2 text-sm text-slate-300">
            <li>✓ 最快响应</li>
            <li>✓ 低成本</li>
            <li>✓ 日常任务</li>
            <li>✓ 本地部署友好</li>
          </ul>
        </div>
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl relative overflow-hidden">
          <div class="absolute top-0 right-0 px-3 py-1 bg-gradient-to-r from-indigo-500 to-purple-500 text-white text-xs font-bold rounded-bl-xl">
            推荐
          </div>
          <div class="text-sm font-semibold text-indigo-600 mb-2">Sonnet 4</div>
          <div class="text-3xl font-black text-slate-900 mb-4">平衡之选</div>
          <ul class="space-y-2 text-sm text-slate-600">
            <li>✓ 优秀性价比</li>
            <li>✓ 代码能力强</li>
            <li>✓ 长上下文</li>
            <li>✓ 适合 Agent</li>
          </ul>
        </div>
        <div class="p-6 bg-gradient-to-br from-amber-500 to-orange-600 text-white rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-amber-200 mb-2">Opus 4</div>
          <div class="text-3xl font-black mb-4">旗舰性能</div>
          <ul class="space-y-2 text-sm text-amber-100">
            <li>✓ 最强推理</li>
            <li>✓ 复杂任务</li>
            <li>✓ 200K 上下文</li>
            <li>✓ 深度分析</li>
          </ul>
        </div>
      </div>
      <div class="mt-8 p-4 bg-slate-100 rounded-2xl text-center text-slate-600 text-sm">
        Claude 3.5 Sonnet 是目前最受欢迎的模型，在代码生成、数学推理方面表现出色
      </div>
    </div>
  </section>
</template>