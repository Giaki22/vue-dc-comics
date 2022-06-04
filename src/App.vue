<template>
  <div id="app">
    <OmainHeader></OmainHeader>
    <main></main>
    <footer></footer>
  </div>
</template>

<script>
import OmainHeader from './components/Organisms/OmainHeader.vue'

export default {
  name: 'App',
  components: {
    OmainHeader
}
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
</style>
