<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Harness 系统架构</h2>
      <div class="relative">
        <!-- 层级图 -->
        <div class="flex flex-col items-center gap-4">
          <!-- LLM Layer -->
          <div class="w-full max-w-2xl p-6 bg-gradient-to-r from-indigo-500 to-purple-500 rounded-3xl text-white text-center shadow-xl">
            <div class="text-sm font-semibold opacity-80 mb-2">Foundation</div>
            <div class="text-2xl font-bold">LLM (Claude / GPT-4 / Gemini)</div>
          </div>
          <!-- Arrow -->
          <div class="text-3xl text-slate-400">↑</div>
          <!-- Harness Core -->
          <div class="w-full max-w-2xl p-6 bg-white/80 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-center text-sm font-semibold text-indigo-600 mb-4">Harness Core</div>
            <div class="grid grid-cols-4 gap-4 text-center">
              <div class="p-3 bg-indigo-50 rounded-xl">
                <div class="text-2xl mb-1">🧠</div>
                <div class="text-sm font-semibold text-slate-700">Memory</div>
              </div>
              <div class="p-3 bg-emerald-50 rounded-xl">
                <div class="text-2xl mb-1">⚡</div>
                <div class="text-sm font-semibold text-slate-700">Skills</div>
              </div>
              <div class="p-3 bg-amber-50 rounded-xl">
                <div class="text-2xl mb-1">🔧</div>
                <div class="text-sm font-semibold text-slate-700">Tools</div>
              </div>
              <div class="p-3 bg-rose-50 rounded-xl">
                <div class="text-2xl mb-1">🛡️</div>
                <div class="text-sm font-semibold text-slate-700">Security</div>
              </div>
            </div>
          </div>
          <!-- Arrow -->
          <div class="text-3xl text-slate-400">↑</div>
          <!-- Execution Loop -->
          <div class="w-full max-w-2xl p-6 bg-slate-900 text-white rounded-3xl shadow-xl">
            <div class="text-center text-sm font-semibold text-slate-400 mb-4">Execution Loop</div>
            <div class="flex items-center justify-center gap-4 text-sm">
              <span class="px-4 py-2 bg-slate-700 rounded-full">Plan</span>
              <span class="text-slate-500">→</span>
              <span class="px-4 py-2 bg-slate-700 rounded-full">Execute</span>
              <span class="text-slate-500">→</span>
              <span class="px-4 py-2 bg-slate-700 rounded-full">Review</span>
              <span class="text-slate-500">→</span>
              <span class="px-4 py-2 bg-indigo-500 rounded-full">Loop</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>