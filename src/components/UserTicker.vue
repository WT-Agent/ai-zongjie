<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了产品经理年终 15 页 PPT 述职大纲"
  },
  {
    "text": "用户 189****9900 获得了技术总监年终架构重构量化总结"
  },
  {
    "text": "用户 131****4455 完成了晋升答辩 10 分钟自我述职演讲"
  },
  {
    "text": "用户 156****7788 生成了市场部门年度 ROI 总结与明年规划"
  },
  {
    "text": "用户 173****3311 取得了向上汇报年终总结 Checklist"
  }
]);
</script>
