<template>
  <main>
      <div class="container">
          <AsignUpButton></AsignUpButton>
          <MsocialNav></MsocialNav>
      </div>
  </main>
</template>

<script>
import AsignUpButton from '../Atoms/AsignUpButton.vue';
import MsocialNav from '../Molecules/MsocialNav.vue';
export default {
    name: "OmainFooter",
    components: { AsignUpButton, MsocialNav }
}
</script>

<style scoped>
main{
    background-color: var(--accent-color);
}
.container{
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-content: center;
    margin: 0 auto;
    max-width: 75rem;
    padding: var(--m);
}
</style>