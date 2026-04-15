<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Memory 机制</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
        <div class="p-6 bg-gradient-to-br from-indigo-500/10 to-indigo-600/5 border border-indigo-200/30 rounded-3xl">
          <div class="text-3xl mb-4">💬</div>
          <div class="text-lg font-bold text-slate-800 mb-2">会话记忆</div>
          <p class="text-sm text-slate-600">短期的当前对话上下文，随着交互动态更新</p>
        </div>
        <div class="p-6 bg-gradient-to-br from-emerald-500/10 to-emerald-600/5 border border-emerald-200/30 rounded-3xl">
          <div class="text-3xl mb-4">📚</div>
          <div class="text-lg font-bold text-slate-800 mb-2">知识库</div>
          <p class="text-sm text-slate-600">长期的结构化知识，支持向量检索和语义搜索</p>
        </div>
        <div class="p-6 bg-gradient-to-br from-amber-500/10 to-amber-600/5 border border-amber-200/30 rounded-3xl">
          <div class="text-3xl mb-4">⚙️</div>
          <div class="text-lg font-bold text-slate-800 mb-2">状态管理</div>
          <p class="text-sm text-slate-600">项目级别的上下文记忆，跨会话保持状态</p>
        </div>
      </div>
      <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
        <div class="text-lg font-bold text-slate-800 mb-4">Memory 工作流程</div>
        <div class="flex items-center justify-between gap-4 text-sm">
          <div class="flex-1 p-4 bg-slate-100 rounded-xl text-center">
            <div class="font-semibold">写入</div>
            <div class="text-slate-500 mt-1">学习新信息</div>
          </div>
          <div class="text-2xl text-slate-400">→</div>
          <div class="flex-1 p-4 bg-slate-100 rounded-xl text-center">
            <div class="font-semibold">索引</div>
            <div class="text-slate-500 mt-1">向量化存储</div>
          </div>
          <div class="text-2xl text-slate-400">→</div>
          <div class="flex-1 p-4 bg-slate-100 rounded-xl text-center">
            <div class="font-semibold">检索</div>
            <div class="text-slate-500 mt-1">语义匹配</div>
          </div>
          <div class="text-2xl text-slate-400">→</div>
          <div class="flex-1 p-4 bg-indigo-100 rounded-xl text-center">
            <div class="font-semibold text-indigo-700">应用</div>
            <div class="text-indigo-500 mt-1">上下文注入</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>