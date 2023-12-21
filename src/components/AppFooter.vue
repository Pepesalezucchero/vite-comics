<script>
export default {
    name: "AppFooter"
}
</script>

<template>
    <section class="container">
        <div class="footer-left">
            <div class="col">
                <ul><h2>DC COMICS</h2>
                    <a href="#"><li>Characters</li></a>
                    <a href="#"><li>Comics</li></a>
                    <a href="#"><li>Movies</li></a>
                    <a href="#"><li>TV</li></a>
                    <a href="#"><li>Games</li></a>
                    <a href="#"><li>Videos</li></a>
                    <a href="#"><li>News</li></a>
                </ul>
                <ul><h2>SHOP</h2>
                    <a href="#"><li>Shop DC</li></a>
                    <a href="#"><li>Shop DC Collectibles</li></a>
                </ul>
            </div>
            <div class="col">
                <ul><h2>DC</h2>
                    <a href="#"><li>Term Of Use</li></a>
                    <a href="#"><li>Privacy policy (New)</li></a>
                    <a href="#"><li>Ad Choices</li></a>
                    <a href="#"><li>Advertising</li></a>
                    <a href="#"><li>Jobs</li></a>
                    <a href="#"><li>Subscriptions</li></a>
                    <a href="#"><li>Talent Workshops</li></a>
                    <a href="#"><li>CPSC Certificates</li></a>
                    <a href="#"><li>Ratings</li></a>
                    <a href="#"><li>Shop Help</li></a>
                    <a href="#"><li>Contact Us</li></a>
                </ul>
            </div>
            <div class="col">
                <ul><h2>SITES</h2>
                    <a href="#"><li>DC</li></a>
                    <a href="#"><li>MAD Magazine</li></a>
                    <a href="#"><li>DC Kids</li></a>
                    <a href="#"><li>DC Universe</li></a>
                    <a href="#"><li>DC Power Visa</li></a>
                </ul>
            </div>
        </div>
        <div class="footer-right">
            <div class="logo-jumbotron">

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../src/styles/partials/variables' as *;
.container {
    min-height: 350px;
    display: flex;
}
.footer-left, .footer-right {
    width: 40%;
}

.footer-left {
    display: flex;
    margin-right: auto;
}

.col {
    width: calc(80% / 3);
    margin-right: auto;
}

h2 {
    color: $white;
    font-size: 20px;
    font-weight: 700;
    margin: 20px 0;
}

a {
    color: $light-grey;
    &:hover {
        color: $white;
    }
}

li {
    font-size: 12px;
    margin: 8px 0;
}

.logo-jumbotron {
    height: 100%;
    width: 100%;
    background-size: cover;
    background-position: center;
    background-image: url(../assets/img/dc-logo-bg.png);
}
</style>