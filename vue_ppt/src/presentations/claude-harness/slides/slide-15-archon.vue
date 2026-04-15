<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <div class="flex items-center gap-4 mb-8">
        <div class="px-4 py-2 bg-gradient-to-r from-indigo-500 to-purple-500 text-white text-sm font-bold rounded-full">
          17,962 ⭐
        </div>
        <h2 class="text-4xl font-extrabold text-slate-900">Archon</h2>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-indigo-600 mb-3">首个开源 Harness Builder</div>
            <p class="text-slate-600 leading-relaxed">
              Archon 是专门为 AI coding 设计的开源 harness 构建器，旨在让 AI 编程变得可预测和可重复。它提供了完整的能力框架，包括 Skills 注册、工具调用和执行监控。
            </p>
          </div>
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-emerald-600 mb-3">核心特性</div>
            <ul class="space-y-2 text-slate-600">
              <li>• <strong>确定性执行</strong> - 相同的输入产生相同的输出</li>
              <li>• <strong>可重复性</strong> - 可以复现任何之前的执行结果</li>
              <li>• <strong>高度可配置</strong> - 根据需求定制 harness 行为</li>
              <li>• <strong>丰富的工具生态</strong> - 支持多种外部工具集成</li>
            </ul>
          </div>
        </div>
        <div class="p-6 bg-slate-900 text-slate-100 rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-slate-400 mb-4">快速开始</div>
          <pre class="font-mono text-sm leading-relaxed"><code><span class="text-slate-400"># Clone the repository</span>
<span class="text-emerald-400">git clone</span> https://github.com/ColeAm00/Archon
<span class="text-slate-400">cd Archon</span>

<span class="text-slate-400"># Install dependencies</span>
<span class="text-emerald-400">npm install</span>

<span class="text-slate-400"># Run Archon</span>
<span class="text-emerald-400">npm run dev</span></code></pre>
          <div class="mt-6 pt-6 border-t border-slate-700">
            <div class="text-sm text-slate-400">适用场景</div>
            <div class="flex flex-wrap gap-2 mt-3">
              <span class="px-3 py-1 bg-slate-700 rounded-full text-xs">自动化测试</span>
              <span class="px-3 py-1 bg-slate-700 rounded-full text-xs">代码审查</span>
              <span class="px-3 py-1 bg-slate-700 rounded-full text-xs">文档生成</span>
              <span class="px-3 py-1 bg-slate-700 rounded-full text-xs">持续集成</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>