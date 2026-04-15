<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Execution Loop 执行循环</h2>
      <div class="flex items-center justify-center mb-12">
        <div class="relative w-full max-w-3xl">
          <!-- 循环图示 -->
          <div class="flex items-center justify-center gap-8">
            <div class="flex flex-col items-center gap-3">
              <div class="w-28 h-28 rounded-full bg-gradient-to-br from-indigo-500 to-purple-500 flex items-center justify-center shadow-xl">
                <span class="text-white text-4xl font-bold">1</span>
              </div>
              <div class="text-center">
                <div class="font-bold text-slate-800">Plan</div>
                <div class="text-sm text-slate-500">规划任务</div>
              </div>
            </div>
            <div class="text-3xl text-indigo-400">→</div>
            <div class="flex flex-col items-center gap-3">
              <div class="w-28 h-28 rounded-full bg-gradient-to-br from-emerald-500 to-teal-500 flex items-center justify-center shadow-xl">
                <span class="text-white text-4xl font-bold">2</span>
              </div>
              <div class="text-center">
                <div class="font-bold text-slate-800">Execute</div>
                <div class="text-sm text-slate-500">执行操作</div>
              </div>
            </div>
            <div class="text-3xl text-emerald-400">→</div>
            <div class="flex flex-col items-center gap-3">
              <div class="w-28 h-28 rounded-full bg-gradient-to-br from-amber-500 to-orange-500 flex items-center justify-center shadow-xl">
                <span class="text-white text-4xl font-bold">3</span>
              </div>
              <div class="text-center">
                <div class="font-bold text-slate-800">Review</div>
                <div class="text-sm text-slate-500">检查结果</div>
              </div>
            </div>
          </div>
          <!-- 循环箭头 -->
          <div class="absolute top-1/2 right-0 transform translate-x-1/2 -translate-y-1/2">
            <div class="text-4xl text-slate-400">↻</div>
          </div>
        </div>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-indigo-600 mb-2">Plan 阶段</div>
          <ul class="text-sm text-slate-600 space-y-1">
            <li>• 分析用户意图</li>
            <li>• 分解任务步骤</li>
            <li>• 选择合适的 Skills</li>
          </ul>
        </div>
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-emerald-600 mb-2">Execute 阶段</div>
          <ul class="text-sm text-slate-600 space-y-1">
            <li>• 调用 Tools 执行</li>
            <li>• 读写 Memory</li>
            <li>• 生成响应内容</li>
          </ul>
        </div>
        <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
          <div class="text-sm font-semibold text-amber-600 mb-2">Review 阶段</div>
          <ul class="text-sm text-slate-600 space-y-1">
            <li>• 验证输出质量</li>
            <li>• 检查安全边界</li>
            <li>• 决定是否继续循环</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>