<template>
  <ul>
      <li v-for="(item, i) in navItems" :key="i" :class="{active: navItems[i].active}"><a :href="navItems.link">{{navItems[i].text}}</a></li>
  </ul>
</template>

<script>
export default {
    name: 'MmainNav',
    data() {
        return {
            navItems: [
                {
                    text: "CHARACTERS",
                    link: '#',
                    active: false,
                },
                {
                    text: "COMICS",
                    link: '#',
                    active: true,
                },
                {
                    text: "MOVIES",
                    link: '#',
                    active: false,
                },
                {
                    text: "TV",
                    link: '#',
                    active: false,
                },
                {
                    text: "GAMES",
                    link: '#',
                    active: false,
                },
                {
                    text: "COLLECTIBLES",
                    link: '#',
                    active: false,
                },
                {
                    text: "VLOGS",
                    link: '#',
                    active: false,
                },
                {
                    text: "FANS",
                    link: '#',
                    active: false,
                },
                {
                    text: "NEWS",
                    link: '#',
                    active: false,
                },
                {
                    text: "SHOP",
                    link: '#',
                    active: false,
                }
            ]
        }
    },
}
</script>

<style scoped>
ul{
    display: flex;
    flex-flow: row nowrap;
    gap: var(--s);
    list-style: none;
}
li{
    color: var(--secondary-text-color);
    font-size: 12px;
    font-weight: 700;
    border-bottom: 3px solid transparent;
    transition: all .3s ease-out;
}
.active, li:hover{
    border-bottom-color: var(--primary-color);
    color: var(--primary-color);
    cursor: pointer;
}
</style>