<script>
export default {
    name: "AppBuySection",
    data() {
        return {
            buys: [
                {
                    text:"digital comics",
                    url:"#",
                    img:".."
                },
                {
                    text:"dc merchandise",
                    url:"#",
                    img:"../assets/img/buy-comics-digital-comics.png"
                },
                {
                    text:"subscription",
                    url:"#",
                    img:"../assets/img/buy-comics-digital-comics.png"
                },
                {
                    text:"comic shop locator",
                    url:"#",
                    img:"../assets/img/buy-comics-digital-comics.png"
                },
                {
                    text:"dc power visa",
                    url:"#",
                    img:"../assets/img/buy-comics-digital-comics.png"
                },
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
}

img {
    width: 50px;
    vertical-align: middle;
    margin-right: 15px;
}

span {
    color: $white;
    text-transform: uppercase;
}
</style>