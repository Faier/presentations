<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Skills 系统</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-indigo-600 mb-3">什么是 Skills</div>
            <p class="text-slate-600 leading-relaxed">
              Skills 是封装好的能力单元，定义了 AI 可以执行的操作模式。每个 Skill 包含触发条件、执行逻辑和输出格式。
            </p>
          </div>
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-emerald-600 mb-3">核心特点</div>
            <ul class="space-y-2 text-slate-600">
              <li>• <strong>声明式</strong> - 通过配置而非代码定义</li>
              <li>• <strong>可组合</strong> - 多个 Skills 可以协同工作</li>
              <li>• <strong>可测试</strong> - 内置测试和验证机制</li>
            </ul>
          </div>
        </div>
        <div class="p-6 bg-slate-900 text-slate-100 rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-slate-400 mb-4">示例：Skill 定义</div>
          <pre class="font-mono text-sm leading-relaxed overflow-x-auto"><code><span class="text-emerald-400">name:</span> <span class="text-sky-300">code-review</span>
<span class="text-emerald-400">trigger:</span> <span class="text-amber-300">/review</span>
<span class="text-emerald-400">actions:</span>
  <span class="text-slate-400">-</span> <span class="text-sky-300">fetch-diff</span>
  <span class="text-slate-400">-</span> <span class="text-sky-300">analyze-patterns</span>
  <span class="text-slate-400">-</span> <span class="text-sky-300">generate-report</span>
<span class="text-emerald-400">output:</span> <span class="text-amber-300">markdown</span></code></pre>
        </div>
      </div>
    </div>
  </section>
</template>