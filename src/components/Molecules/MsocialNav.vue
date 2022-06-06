<template>
    <main>
        <h2>FOLLOW US</h2>
        <img src="../../assets/img/footer-facebook.png" alt="404">
        <img src="../../assets/img/footer-twitter.png" alt="404">
        <img src="../../assets/img/footer-youtube.png" alt="404">
        <img src="../../assets/img/footer-pinterest.png" alt="404">
        <img src="../../assets/img/footer-periscope.png" alt="404">
    </main>
</template>

<script>
export default {
    name: 'MsocialNav'
}
</script>

<style lang='scss' scoped>
main{
    display: flex;
    flex-flow: row nowrap;
    gap: var(--xs);

    h2{
        color: var(--primary-color);
        font-size: 1rem;
    }

    img{
        width: var(--s);
        height: var(--s);
    }
    img:hover{
        cursor: pointer;
        }
}
</style>