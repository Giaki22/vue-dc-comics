<template>
  <div id="app">
    <OmainHeader></OmainHeader>
    <OmainMain></OmainMain>
    <footer></footer>
  </div>
</template>

<script>
import OmainHeader from './components/Organisms/OmainHeader.vue'
import OmainMain from './components/Organisms/OmainMain.vue'

export default {
  name: 'App',
  components: {
    OmainHeader,
    OmainMain
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
