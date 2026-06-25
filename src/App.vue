<template>
  <div id="app">
    <a-config-provider :locale="zhCN">
      <BasicLayout />
    </a-config-provider>
  </div>
</template>

<script setup lang="ts">
import BasicLayout from './layouts/BasicLayout.vue'
import { healthUsingGet } from '@/api/mainController.ts'
import { provide } from 'vue'
import zhCN from 'ant-design-vue/es/locale/zh_CN'
import dayjs from 'dayjs'
import 'dayjs/locale/zh-cn'
import { onMounted } from 'vue'
dayjs.locale('zh-cn')

onMounted(() => {
  document.body.contentEditable = 'false'
})
</script>

<style scoped>
#app {
  user-select: none;
}
</style>
