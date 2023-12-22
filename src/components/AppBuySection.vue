<script>
export default {
    name: "AppBuySection",
    data() {
        return {
            buys: [
                {
                    text:"digital comics",
                    url:"#",
                    img:"img/buy-comics-digital-comics.png"
                },
                {
                    text:"dc merchandise",
                    url:"#",
                    img:"img/buy-comics-merchandise.png"
                },
                {
                    text:"subscription",
                    url:"#",
                    img:"img/buy-comics-subscriptions.png"
                },
                {
                    text:"comic shop locator",
                    url:"#",
                    img:"img/buy-comics-shop-locator.png"
                },
                {
                    text:"dc power visa",
                    url:"#",
                    img:"img/buy-dc-power-visa.svg"
                }
            ]
        }
    }
}
</script>

<template>
    <section class="container">
        <ul>
            <li v-for="(buy, i) in buys" :key="i">
                <a href="#">
                   <img :src=buy.img :alt= buy.text> 
                   <span>{{ buy.text }}</span>
                </a>
            </li>

            <img src="" alt="">
        </ul>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.container {
    min-height: 175px;
    display: flex;
    justify-content: space-between;
}

ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin: 0 35px;
}

img {
    height: 70px;
    vertical-align: middle;
    margin-right: 15px;
}

span {
    color: $white;
    text-transform: uppercase;
}
</style>