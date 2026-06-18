<template>
  <div id="homePage">
    <div style="text-align: center; margin-top: 100px">
      <h1>欢迎来到云图库！</h1>
      <p>这是一个基于Vue3和Ant Design Vue构建的图片管理平台。</p>
      <p>请使用顶部导航栏浏览不同的功能模块。</p>
    </div>
  </div>
</template>

<script setup lang="ts">
import BasicLayout from '../layouts/BasicLayout.vue'
import { healthUsingGet } from '@/api/mainController.ts'
</script>

<style scoped>
#homePage {
}
</style>
