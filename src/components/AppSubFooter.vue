<script>
export default {
    name: "AppSubFooter"
}
</script>

<template>
    <section class="container">
        <div class="btn">
            <button>SIGN-UP NOW!</button>
        </div>
        <div class="social">
            <h1>FOLLOW US</h1>
            <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
            <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

.container {
    min-height: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.social {
    display: flex;
    align-items: center;
}

.btn button {
    padding: 12px;
    border: 3px solid $blue;
    background-color: $grey;
    cursor: pointer;
    color: $white;
    font-size: 18px;
    font-weight: 500;
}

h1 {
    color: $blue;
    font-size: 20px;
    font-weight: 500;
}

a {
    margin-left: 20px;
}

img {
    border-radius: 50%;

    &:hover {
        box-shadow: 0px 0px 25px 10px #9b97973f;
    }
}

</style>