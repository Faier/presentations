<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">什么是 Agent Harness</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="space-y-6">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-2xl font-bold text-indigo-600 mb-3">🤔 传统 AI 助手的问题</div>
            <ul class="space-y-3 text-slate-600">
              <li class="flex items-start gap-3">
                <span class="text-rose-500 mt-1">✗</span>
                <span>单次交互，缺乏持续性</span>
              </li>
              <li class="flex items-start gap-3">
                <span class="text-rose-500 mt-1">✗</span>
                <span>无法访问外部工具和 API</span>
              </li>
              <li class="flex items-start gap-3">
                <span class="text-rose-500 mt-1">✗</span>
                <span>无法记住对话历史</span>
              </li>
              <li class="flex items-start gap-3">
                <span class="text-rose-500 mt-1">✗</span>
                <span>无法执行复杂的多步骤任务</span>
              </li>
            </ul>
          </div>
        </div>
        <div class="space-y-6">
          <div class="p-6 bg-gradient-to-br from-indigo-500/10 to-emerald-400/10 border border-indigo-200/30 rounded-3xl shadow-xl">
            <div class="text-2xl font-bold text-indigo-600 mb-3">✨ Harness 的解决方案</div>
            <ul class="space-y-3 text-slate-700">
              <li class="flex items-start gap-3">
                <span class="text-emerald-500 mt-1">✓</span>
                <span><strong>Skills</strong> - 可复用的能力封装</span>
              </li>
              <li class="flex items-start gap-3">
                <span class="text-emerald-500 mt-1">✓</span>
                <span><strong>Memory</strong> - 持久化上下文</span>
              </li>
              <li class="flex items-start gap-3">
                <span class="text-emerald-500 mt-1">✓</span>
                <span><strong>Tools</strong> - 调用外部系统</span>
              </li>
              <li class="flex items-start gap-3">
                <span class="text-emerald-500 mt-1">✓</span>
                <span><strong>Security</strong> - 权限与边界控制</span>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>