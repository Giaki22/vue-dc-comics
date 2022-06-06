<template>
<div class="lists">
    <ul v-for="(obj, i) in lists" :key="i">{{obj.title}}
      <li v-for="(listLink, index) in lists[i].links" :key="index">{{listLink}}</li>
    </ul>
</div>
</template>

<script>
export default {
    name:'MlinksNav',
    data() {
        return {
            lists: [
                {
                    title: 'DC COMICS',
                    links: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
                },
                {
                    title: 'SHOP',
                    links: ['Shop DC', 'Shop DC Collectibles']
                },
                {
                    title: 'DC',
                    links: ['Terms of Use', 'Privacy Policy (New)', 'Ad Choises', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
                },
                {
                    title: 'SITES',
                    links: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
                },
            ]
        }
    }
}
</script>

<style scoped>
.lists{
    display: flex;
    flex-flow: column wrap;
    gap: var(--m);
    width: 50%;
    padding: var(--m);
    max-height: 25rem;
}
ul{
    color: var(--primary-text-color);
    display: flex;
    flex-flow: column wrap;
    list-style: none;
    gap: var(--xs);
    font-size: .9375rem;
    font-weight: 300;
}
li{
    color: rgba(255, 255, 255, 0.5);
    font-size: var(--xs);
}
li:hover{
    cursor: pointer;
    color: var(--accent-text-color);
}
</style>