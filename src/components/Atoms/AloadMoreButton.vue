<template>
  <button>{{ text }}</button>
</template>

<script>
export default {
    name:'AloadMoreButton',
    props: {
        text: String
    }
}
</script>

<style>
button{
    background-color: var(--primary-color);
    border: none;
    box-shadow: none;
    color: var(--primary-text-color);
    padding: var(--xs);
    font-weight: 700;;
}
</style>