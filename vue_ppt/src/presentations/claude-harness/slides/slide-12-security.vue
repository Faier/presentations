<script setup lang="ts">
defineProps<{ isActive?: boolean; isPreview?: boolean }>()
</script>

<template>
  <section class="slide-shell">
    <div class="container mx-auto max-w-5xl px-6 py-12">
      <h2 class="text-4xl font-extrabold text-slate-900 mb-8">Security 安全机制</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="flex items-center gap-4 mb-4">
              <div class="text-3xl">🔐</div>
              <div class="text-xl font-bold text-slate-800">权限控制</div>
            </div>
            <ul class="space-y-2 text-slate-600">
              <li>• 基于角色的访问控制 (RBAC)</li>
              <li>• 细粒度的工具调用授权</li>
              <li>• 操作审计日志完整记录</li>
            </ul>
          </div>
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="flex items-center gap-4 mb-4">
              <div class="text-3xl">🛡️</div>
              <div class="text-xl font-bold text-slate-800">内容安全</div>
            </div>
            <ul class="space-y-2 text-slate-600">
              <li>• 输入过滤与验证</li>
              <li>• 输出内容安全检测</li>
              <li>• 敏感信息自动脱敏</li>
            </ul>
          </div>
        </div>
        <div class="space-y-4">
          <div class="p-6 bg-white/70 backdrop-blur-md border border-slate-200/30 rounded-3xl shadow-xl">
            <div class="flex items-center gap-4 mb-4">
              <div class="text-3xl">⏱️</div>
              <div class="text-xl font-bold text-slate-800">资源限制</div>
            </div>
            <ul class="space-y-2 text-slate-600">
              <li>• 最大执行时间限制</li>
              <li>• 工具调用次数上限</li>
              <li>• 防止无限循环和资源耗尽</li>
            </ul>
          </div>
          <div class="p-6 bg-gradient-to-br from-rose-500/10 to-rose-600/5 border border-rose-200/30 rounded-3xl">
            <div class="flex items-center gap-4 mb-4">
              <div class="text-3xl">🚨</div>
              <div class="text-xl font-bold text-slate-800">异常处理</div>
            </div>
            <ul class="space-y-2 text-slate-700">
              <li>• 自动熔断机制</li>
              <li>• 优雅的失败降级</li>
              <li>• 用户友好的错误提示</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>