<template>
    <main>
        <div class="content">
            <div class="container">
                <MmainContent></MmainContent>
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
import MmainContent from '../Molecules/MmainContent.vue';
import MsecondNav from '../Molecules/MsecondNav.vue';
import MlinksNav from '../Molecules/MlinksNav.vue';
import AbigLogo from '../Atoms/AbigLogo.vue';

export default {
    name: "OmainMain",
    components: { MmainContent, MsecondNav, MlinksNav, AbigLogo }
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
</style>