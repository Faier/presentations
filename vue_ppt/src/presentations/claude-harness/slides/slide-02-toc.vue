<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()

const chapters = [
  { title: 'Claude 概述', desc: '模型家族与能力' },
  { title: 'Harness 概述', desc: '核心概念与价值' },
  { title: '核心组件', desc: 'Skills/Memory/Security' },
  { title: '开源生态', desc: 'Archon/Code Book' },
]
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-bold text-slate-900 mb-8">内容概览</h2>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
        <div v-for="(chapter, i) in chapters" :key="i"
          class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl hover:shadow-2xl transition-all cursor-pointer group">
          <div class="text-3xl font-black text-transparent bg-clip-text bg-gradient-to-r from-indigo-500 to-emerald-400 mb-3">
            {{ String(i + 1).padStart(2, '0') }}
          </div>
          <div class="font-semibold text-slate-800 group-hover:text-indigo-600 transition-colors">
            {{ chapter.title }}
          </div>
          <div class="text-sm text-slate-500 mt-1">{{ chapter.desc }}</div>
        </div>
      </div>
    </div>
  </section>
</template>