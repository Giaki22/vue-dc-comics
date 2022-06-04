<template>
  <ul>
    <li v-for="(item, i) in links" :key="i">
        <img :src="item.img" alt="">
        <h6>{{item.text}}</h6>
    </li>
  </ul>
</template>

<script>
export default {
name: 'MsecondNav',
data() {
    return {
        links: [
            {
                img: require('../../assets/img/buy-comics-digital-comics.png'),
                text: 'DIGITAL COMICS'
            },
            {
                img: require('../../assets/img/buy-comics-merchandise.png'),
                text: 'DC MERCHANDISE'
            },
            {
                img: require('../../assets/img/buy-comics-subscriptions.png'),
                text: 'SUBSCRIPTION'
            },
            {
                img: require('../../assets/img/buy-comics-shop-locator.png'),
                text: 'COMIC SHOP LOCATOR'
            },
            {
                img: require('../../assets/img/buy-dc-power-visa.svg'),
                text: 'DC POWER VISA'
            },
        ]
    }
}
}
</script>

<style scoped>
ul{
    display: flex;
    flex-flow: row nowrap;
    gap: .625rem;
    list-style: none;
    justify-content: space-around;
    align-content: center;
    max-width: 75rem;
}
li{
    display: flex;
    flex-flow: row nowrap;
    color: var(--primary-text-color);
    align-items: center;
    gap: var(--xs);
}
img{
    width: 45px;
    height: 60px;
}
</style>