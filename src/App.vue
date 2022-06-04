<template>
  <div id="app">
    <BasicLogo></BasicLogo>
  </div>
</template>

<script>
import BasicLogo from './components/basicLogo.vue';

export default {
  name: 'App',
  components: {
    BasicLogo
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss'
</style>
