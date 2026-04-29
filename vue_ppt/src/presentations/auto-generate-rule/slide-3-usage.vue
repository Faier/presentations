<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <img src="/solo.png" alt="SOP" class="company-logo" />
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <div class="flex items-center justify-center gap-4 mb-8 flex-wrap">
        <h2 class="text-4xl font-extrabold text-slate-900">一句话生成规则</h2>
        <span class="px-4 py-1.5 rounded-full bg-indigo-100 border border-indigo-300 text-sm font-semibold text-indigo-600 whitespace-nowrap">
          约定 &gt; 配置
        </span>
      </div>

      <!-- Flow: 3 cards with arrows -->
      <div class="flex items-center gap-4 mb-10 flex-wrap justify-center">
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl text-center min-w-[180px] flex-1 max-w-[260px]">
          <div class="text-3xl mb-3">&#128172;</div>
          <div class="text-sm font-semibold text-rose-500 mb-2">你 说</div>
          <p class="text-slate-600 text-sm leading-relaxed">在用药合理性下创建规则，患者过敏史包含青霉素，用药为青霉素钠，进行禁忌提醒</p>
        </div>

        <div class="text-2xl text-slate-300 font-bold flex-shrink-0">&#10132;</div>

        <div class="p-6 bg-gradient-to-br from-indigo-500/10 to-emerald-400/10 border border-indigo-200/30 rounded-3xl text-center min-w-[180px] flex-1 max-w-[260px]">
          <div class="text-3xl mb-3">&#9889;</div>
          <div class="text-sm font-semibold text-indigo-500 mb-2">AI 自动</div>
          <ul class="text-slate-600 text-sm space-y-1 text-left">
            <li>&#8226; 匹配规则类别</li>
            <li>&#8226; 查元数据 + 字典表</li>
            <li>&#8226; 生成 flow_content</li>
          </ul>
        </div>

        <div class="text-2xl text-slate-300 font-bold flex-shrink-0">&#10132;</div>

        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl text-center min-w-[180px] flex-1 max-w-[260px]">
          <div class="text-3xl mb-3">&#9989;</div>
          <div class="text-sm font-semibold text-emerald-500 mb-2">得 到</div>
          <p class="text-slate-600 text-sm leading-relaxed">一条可直接执行的 <strong class="text-slate-900">r_rules 记录</strong></p>
        </div>
      </div>

      <!-- Bottom: Key points -->
      <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
        <div class="p-4 bg-white/60 backdrop-blur-md border border-slate-200/30 rounded-2xl text-center">
          <div class="text-lg font-bold text-indigo-600">触发方式</div>
          <p class="text-sm text-slate-500 mt-1">说"生成规则 / 创建规则"即可</p>
        </div>
        <div class="p-4 bg-white/60 backdrop-blur-md border border-slate-200/30 rounded-2xl text-center">
          <div class="text-lg font-bold text-emerald-600">知识库驱动</div>
          <p class="text-sm text-slate-500 mt-1">6 类字典表 + 集合查询 + 脚本配置</p>
        </div>
        <div class="p-4 bg-white/60 backdrop-blur-md border border-slate-200/30 rounded-2xl text-center">
          <div class="text-lg font-bold text-amber-600">一次确认</div>
          <p class="text-sm text-slate-500 mt-1">展示摘要 → 用户确认 → 写入 Oracle</p>
        </div>
      </div>

      <p class="text-center text-sm text-slate-500 mt-6">你只需描述意图，其余由技能自动推断</p>
    </div>
  </section>
</template>

<style scoped>
.slide-shell {
  display: flex;
  height: 100%;
  width: 100%;
  align-items: center;
  justify-content: center;
  padding: clamp(3rem, 8vw, 7rem);
  background: radial-gradient(120% 140% at 50% 50%, rgba(99, 102, 241, 0.08), transparent 60%),
    #f8fafc;
  position: relative;
}

.company-logo {
  position: absolute;
  top: 1.5rem;
  left: 2rem;
  height: 48px;
  width: auto;
  z-index: 20;
  opacity: 0.85;
}
</style>
