<template>
  <div id="app">
    <button type="button" @click="showDialog = true">ダイアログを表示</button>
    <sample-dialog v-if="showDialog" @close="showDialog = false" />
  </div>
</template>

<script>
import SampleDialog from './components/SampleDialog.vue'

export default {
  name: 'app',
  components: {
    SampleDialog
  },
  data () {
    return {
      showDialog: false
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
