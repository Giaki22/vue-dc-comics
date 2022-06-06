<template>
<main>
    <img :src="image" alt="Image">
    <h6> {{title}} </h6>
</main>
</template>

<script>
export default {
    name: 'AcomicAndTitle',
    props: {
        title: String,
        image: String
    }
}
</script>

<style lang="scss" scoped>
main{
    display: flex;
    flex-flow: column nowrap;
    gap: .625rem;
    padding: .625rem;
    img{
        width: 100%;
        height: auto;
        aspect-ratio: 1/1;
        object-fit: cover;
        object-position: top;
        transition: box-shadow .2s ease-out;
    }
    h6{
        color: var(--primary-text-color);
        text-transform: uppercase;
        font-weight: 400;
        transition: color .2s ease-out;
    }
    &:hover {
        &>img{
            box-shadow: 15px 15px 49px 5px rgba(0,0,0,0.7);
            cursor: pointer;
        }
        &>h6{
            color: var(--accent-text-color);
        }
    } 
}
</style>