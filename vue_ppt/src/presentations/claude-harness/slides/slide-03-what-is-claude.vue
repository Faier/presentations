<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Claude 是什么</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-indigo-600 mb-3">Anthropic 的 AI 助手</div>
            <p class="text-slate-600 leading-relaxed">
              Claude 是由 Anthropic 公司开发的大型语言模型，主打安全性和有用性。采用 Constitutional AI 和 RLHF 技术训练，强调对人类意图的理解和遵循。
            </p>
          </div>
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-emerald-600 mb-3">多模态能力</div>
            <p class="text-slate-600 leading-relaxed">
              支持文本、图像、文档理解。可以阅读 PDF、分析图表、生成代码、创作内容。是目前最强的通用 AI 助手之一。
            </p>
          </div>
        </div>
        <div class="flex items-center justify-center">
          <div class="p-8 bg-gradient-to-br from-indigo-500/10 to-emerald-400/10 rounded-3xl border border-indigo-200/30">
            <div class="text-8xl mb-4">🤖</div>
            <div class="text-center font-bold text-slate-700">Anthropic Claude</div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>