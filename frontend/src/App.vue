<template>
  <div class="loading">
    <p>正在连接到 DeepSeek...</p>
  </div>
</template>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  window.location.href = 'https://chat.deepseek.com/'
})
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body, #app {
  width: 100%;
  height: 100%;
}

.loading {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  font-size: 16px;
  color: #333;
  background: #fff;
}
</style>