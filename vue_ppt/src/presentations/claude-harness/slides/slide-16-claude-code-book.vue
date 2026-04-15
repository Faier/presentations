<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <div class="flex items-center gap-4 mb-8">
        <div class="px-4 py-2 bg-gradient-to-r from-amber-500 to-orange-500 text-white text-sm font-bold rounded-full">
          2,698 ⭐
        </div>
        <h2 class="text-4xl font-extrabold text-slate-900">《御舆：解码 Agent Harness》</h2>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-amber-600 mb-3">42万字深度剖析</div>
            <p class="text-slate-600 leading-relaxed">
              这是一本关于 Claude Code 架构的深度剖析指南，作者是 lintsinghua。内容涵盖从对话循环到构建自己的 Agent Harness 的完整知识体系。
            </p>
          </div>
          <div class="p-6 bg-gradient-to-br from-amber-500/10 to-orange-500/10 border border-amber-200/30 rounded-3xl">
            <div class="text-lg font-bold text-slate-800 mb-4">内容结构（15章）</div>
            <div class="grid grid-cols-2 gap-3 text-sm">
              <div class="p-3 bg-white/50 rounded-xl">第一章：Claude Code 概述</div>
              <div class="p-3 bg-white/50 rounded-xl">第二章：Agent 循环机制</div>
              <div class="p-3 bg-white/50 rounded-xl">第三章：Skills 系统</div>
              <div class="p-3 bg-white/50 rounded-xl">第四章：Memory 管理</div>
              <div class="p-3 bg-white/50 rounded-xl">第五章：Tool 调用</div>
              <div class="p-3 bg-white/50 rounded-xl">... 更多章节</div>
            </div>
          </div>
        </div>
        <div class="p-6 bg-slate-900 text-slate-100 rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-slate-400 mb-4">书籍特色</div>
          <ul class="space-y-3 text-slate-300">
            <li class="flex items-start gap-3">
              <span class="text-amber-400 mt-1">★</span>
              <span>深入源码分析，揭秘 Claude Code 内部实现</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-amber-400 mt-1">★</span>
              <span>丰富的图示和流程图，帮助理解复杂概念</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-amber-400 mt-1">★</span>
              <span>实战导向，包含大量可运行的代码示例</span>
            </li>
            <li class="flex items-start gap-3">
              <span class="text-amber-400 mt-1">★</span>
              <span>中文原创，对国内开发者更友好</span>
            </li>
          </ul>
          <div class="mt-6 pt-6 border-t border-slate-700">
            <a href="https://github.com/lintsinghua/claude-code-book" class="text-indigo-400 hover:underline text-sm">
              GitHub: lintsinghua/claude-code-book →
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>