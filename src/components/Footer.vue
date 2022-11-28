<template>
  <a-layout-footer style="text-align: center">
    <a-back-top />
    <span>Code with by <a target="_blank" href="https://blog.aidengrong">番茄酱</a></span>
    <span v-if="beian">
      | <a target="_blank" href="http://beian.miit.gov.cn/">{{ beian }}</a></span
    >
  </a-layout-footer>
</template>

<script setup>
import { ref } from 'vue'
const beian = ref(window.Config.beian)
</script>
