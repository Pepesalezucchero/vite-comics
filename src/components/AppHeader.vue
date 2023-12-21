<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text:"characters",
                    url:"#",
                    current: false
                },
                {
                    text:"comics",
                    url:"#",
                    current: true
                },
                {
                    text:"movies",
                    url:"#",
                    current: false
                },
                {
                    text:"tv",
                    url:"#",
                    current: false
                },
                {
                    text:"games",
                    url:"#",
                    current: false
                },
                {
                    text:" collectibles",
                    url:"#",
                    current: false
                },
                {
                    text:"videos",
                    url:"#",
                    current: false
                },
                {
                    text:"fans",
                    url:"#",
                    current: false
                },
                {
                    text:"news",
                    url:"#",
                    current: false
                },
                {
                    text:"shop",
                    url:"#",
                    current: false
                }
            ]
        }
    }
}
</script>

<template>
    <nav class="container">
        <div id="logo">
            <a href="#"><img src="../assets/img/dc-logo.png" alt="Logo pagina DC universe"></a>
        </div>
        <div class="right-navbar">
            <ul>
                <li v-for="link in links">
                    <a :href="link.url" :class="link.current ? 'selected' : ''">
                        {{ link.text }}
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
.container {
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 20px 0;
}
#logo {
    width: 7%;
    display: flex;
    align-items: center;
    img {
        width: 100%;
    }
}
.right-navbar {
    width: 93%;
    display: flex;
    justify-content: end;
    ul {
        display: flex;
        align-items: center;
        a {
            text-transform: uppercase;
            font-weight: 500;
            color: $grey;
            margin-left: 25px;

            &.selected,
            &:hover {
                color: $blue;
                border-bottom: $blue 1px solid;
            }
        }
    }
}
</style>