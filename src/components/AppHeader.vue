<script>
export default {
    name: "AppHeader"
}
</script>

<template>
    <nav class="container">
        <div id="logo">
            <a href="#"><img src="../assets/img/dc-logo.png" alt="Logo pagina DC universe"></a>
        </div>
        <div class="right-navbar">
            <ul>
                <a href="#"><li>characters</li></a>
                <a href="#" class="selected"><li>comics</li></a>
                <a href="#"><li>movies</li></a>
                <a href="#"><li>tv</li></a>
                <a href="#"><li>games</li></a>
                <a href="#"><li>collectibles</li></a>
                <a href="#"><li>videos</li></a>
                <a href="#"><li>fans</li></a>
                <a href="#"><li>news</li></a>
                <a href="#"><li>shop</li></a>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
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
            color: $tertiary;
            margin-left: 25px;

            &.selected,
            &:hover {
                color: $primary;
            }
        }
    }
}
</style>