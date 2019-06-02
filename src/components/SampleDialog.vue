<template>
  <div class="wrapper">
    <div class="dialog">
      <h1>ダイアログ</h1>
      <p>コンテンツ</p>
      <button type="button" @click="close()">閉じる</button>
    </div>
  </div>
</template>

<script>
  export default {
    methods: {
      close() {
        this.$emit('close')
      }
    }
  }
</script>

<style scoped>
  .wrapper {
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 1.0);
  }

  .dialog {
    background-color: #dbdce1;
  }
</style>