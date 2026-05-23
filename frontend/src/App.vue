<template>
  <div class="app-container">
    <iframe 
      id="deepseek-iframe" 
      src="https://chat.deepseek.com/" 
      frameborder="0"
    ></iframe>
  </div>
</template>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body, #app, .app-container {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

#deepseek-iframe {
  width: 100%;
  height: 100%;
  border: none;
}
</style>
