
<template>
  <div>
      <h1 class="demo_title">Demo</h1>
      <div class="demo_containt">
        <Menu></Menu>
        <div class="demo_view"><nuxt /></div>
      </div>
  </div>
</template>

<script>
import Menu from '@/components/header/Menu';
export default {
  components: Menu
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
html {
  /* font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif; */
  font-family: '游ゴシック体', YuGothic, '游ゴシック Medium', 'Yu Gothic Medium',
    '游ゴシック', 'Yu Gothic', 'メイリオ', sans-serif;
  color: #606266;
  min-width: 1400px;
}

.demo_title {
  background: beige;
  padding-left: 20px;
}

.demo_containt {
  display: flex;
}

.demo_view {
    width: 100%;
    height: calc(100vh - 52px);
  }
</style>
