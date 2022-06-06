<template>
    <main>
        <AmainJumbo></AmainJumbo>
        <div class="content">
            <div class="container relative">
                <AloadMoreButton :text="'CURRENT SERIES'" class="currentSeries"></AloadMoreButton>
                <McomicsNav></McomicsNav>
                <AloadMoreButton :text="'LOAD MORE'" class="loadMore"></AloadMoreButton>
            </div>
        </div>
        <nav class="nav">
            <div class="container">
                <MsecondNav></MsecondNav>
            </div>
        </nav>
        <footer>
            <div class="container footer">
                <MlinksNav></MlinksNav>
                <AbigLogo></AbigLogo>
            </div>
        </footer>
    </main>
</template>

<script>
import MsecondNav from '../Molecules/MsecondNav.vue';
import MlinksNav from '../Molecules/MlinksNav.vue';
import AbigLogo from '../Atoms/AbigLogo.vue';
import AmainJumbo from '../Atoms/AmainJumbo.vue';
import McomicsNav from '../Molecules/McomicsNav.vue';
import AloadMoreButton from '../Atoms/AloadMoreButton.vue';

export default {
    name: "OmainMain",
    components: { MsecondNav, MlinksNav, AbigLogo, AmainJumbo, McomicsNav, AloadMoreButton}
}
</script>

<style scoped>
main{
    display: flex;
    flex-flow: column nowrap;
}
.content{
    padding: var(--m);
    background-color: var(--secondary-color);
}
nav{
    padding: var(--m);
    background-color: var(--primary-color);
}
footer{
    background-image: url('../../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    max-height: 25rem;
    overflow: hidden;
}
.container{
    margin: 0 auto;
    max-width: 75rem;
    padding: 0 var(--m);
}
.container.footer{
    display: flex;
    flex-flow: row nowrap;
}
.relative{
    position: relative;
    display: flex;
    flex-flow: column nowrap;
    justify-content: center;
    align-items: center;
}
.currentSeries{
    position: absolute;
    top: -3.75rem;
    left: 1.25rem;
    width: 9.375rem;
}
.loadMore{
    width: 12.5rem;
}
.loadMore:hover{
    cursor: pointer;
}
</style>