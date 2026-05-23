<template>
  <div class="container">
    <div class="content">
      <h1>DeepSeek Chat Desktop</h1>
      <p class="hint">正在打开浏览器...</p>
      <p class="sub">如果浏览器未自动打开，请手动访问：</p>
      <a class="link" href="#!" @click.prevent="openBrowser">https://chat.deepseek.com</a>
    </div>
  </div>
</template>

<script setup>
function openBrowser() {
  window.location.href = 'https://chat.deepseek.com/'
}
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

.container {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
}

.content {
  text-align: center;
  color: #fff;
  padding: 40px;
}

h1 {
  font-size: 28px;
  margin-bottom: 16px;
  font-weight: 600;
}

.hint {
  font-size: 18px;
  margin-bottom: 12px;
  opacity: 0.9;
}

.sub {
  font-size: 14px;
  opacity: 0.7;
  margin-bottom: 8px;
}

.link {
  color: #fff;
  font-size: 16px;
  text-decoration: underline;
  opacity: 0.8;
  cursor: pointer;
}

.link:hover {
  opacity: 1;
}
</style>