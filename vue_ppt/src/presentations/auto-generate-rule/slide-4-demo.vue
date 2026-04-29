<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <img src="/solo.png" alt="SOP" class="company-logo" />
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <div class="text-center mb-8">
        <span class="inline-block px-4 py-1 rounded-full bg-amber-100 text-amber-700 text-sm font-semibold mb-3">真实案例</span>
        <h2 class="text-4xl font-extrabold text-slate-900">高风险手术脑梗死预警</h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Left: Input -->
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-rose-500 mb-3">&#128172; 输入</div>
            <p class="text-slate-700 leading-relaxed">
              在高风险手术下，检查结果包含<strong>脑梗死</strong>且手术医嘱为<strong>主动脉瓣生物瓣膜置换术</strong>，则进行提醒
            </p>
          </div>

          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="text-xl font-bold text-indigo-600 mb-3">&#9889; AI 解析</div>
            <ul class="space-y-2 text-slate-600 text-sm">
              <li class="flex items-start gap-2">
                <span class="text-indigo-500 mt-0.5">&#9654;</span>
                <span>手术不为空 → 检查结果文本包含脑梗死 → 手术 = 主动脉瓣生物瓣膜置换术</span>
              </li>
              <li class="flex items-start gap-2">
                <span class="text-indigo-500 mt-0.5">&#9654;</span>
                <span>结果类型：消息提醒</span>
              </li>
              <li class="flex items-start gap-2">
                <span class="text-indigo-500 mt-0.5">&#9654;</span>
                <span>规则名称：高风险手术脑梗死预警</span>
              </li>
            </ul>
          </div>
        </div>

        <!-- Right: Output -->
        <div class="p-6 bg-slate-900 text-slate-100 rounded-3xl shadow-xl flex flex-col">
          <div class="text-sm font-semibold text-slate-400 mb-4">生成的 flow_content</div>
          <pre class="font-mono text-sm leading-relaxed overflow-x-auto flex-1"><code><span class="text-sky-300">"lineList"</span>: [
    {<span class="text-emerald-400">"from"</span>: <span class="text-amber-300">"cond_01"</span>, <span class="text-emerald-400">"to"</span>: <span class="text-amber-300">"cond_02"</span>},
    {<span class="text-emerald-400">"from"</span>: <span class="text-amber-300">"cond_02"</span>, <span class="text-emerald-400">"to"</span>: <span class="text-amber-300">"cond_03"</span>},
    {<span class="text-emerald-400">"from"</span>: <span class="text-amber-300">"cond_03"</span>, <span class="text-emerald-400">"to"</span>: <span class="text-amber-300">"result"</span>}
  ],
  <span class="text-sky-300">"nodeList"</span>: [
    {<span class="text-emerald-400">"name"</span>: <span class="text-amber-300">"手术 不为空"</span>},
    {<span class="text-emerald-400">"name"</span>: <span class="text-amber-300">"检查结果文本 包含 脑梗死"</span>},
    {<span class="text-emerald-400">"name"</span>: <span class="text-amber-300">"手术 等于 主动脉瓣..."</span>},
    {<span class="text-emerald-400">"name"</span>: <span class="text-amber-300">"禁忌类别 等于 消息提醒"</span>}
  ]</code></pre>

          <!-- Warning box -->
          <div class="mt-4 p-4 bg-rose-500/10 border border-rose-300/30 rounded-2xl">
            <p class="text-sm text-rose-300 leading-relaxed">
              &#9888; 患者存在脑梗死病史，做主动脉瓣生物瓣膜置换术存在高风险，需评估获益与风险。
            </p>
          </div>
        </div>
      </div>
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
  background: radial-gradient(120% 140% at 85% 10%, rgba(99, 102, 241, 0.12), transparent 55%),
    radial-gradient(90% 120% at 10% 90%, rgba(239, 68, 68, 0.08), transparent 60%),
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
