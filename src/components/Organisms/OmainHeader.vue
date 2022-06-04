<template>
    <header>
        <AbasicLogo></AbasicLogo>
        <MmainNav></MmainNav>
    </header>
</template>

<script>
import AbasicLogo from '../Atoms/AbasicLogo.vue';
import MmainNav from '../Molecules/MmainNav.vue';

export default {
    name: 'OmainHeader',
    components: { AbasicLogo, MmainNav }
}
</script>

<style>
header{
    margin: auto;
    max-width: 75rem;
    padding: 0 var(--m);
    display: flex;
    flex-flow: row nowrap;
    justify-content: space-between;
    align-items: center;
    height: 6.25rem;
    line-height: 6.25rem;
}
</style>