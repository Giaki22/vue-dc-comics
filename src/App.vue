<template>
  <div id="app">
    <OmainHeader></OmainHeader>
    <OmainMain></OmainMain>
    <OmainFooter></OmainFooter>
  </div>
</template>

<script>
import OmainHeader from './components/Organisms/OmainHeader.vue'
import OmainMain from './components/Organisms/OmainMain.vue'
import OmainFooter from './components/Organisms/OmainFooter.vue'

export default {
  name: 'App',
  components: {
    OmainHeader,
    OmainMain,
    OmainFooter
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
