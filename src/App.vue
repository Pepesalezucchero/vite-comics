<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppBuySection from './components/AppBuySection.vue'
import AppFooter from './components/AppFooter.vue'
import AppSubFooter from './components/AppSubFooter.vue'

export default {
  components: {
    AppHeader,
    AppMain,
    AppBuySection,
    AppFooter,
    AppSubFooter
  }
}
</script>

<template>
  <div class="container">
    <AppHeader />
  </div>
  <main>
    <div class="main-jumbotron">

    </div>
    <div class="main-backgound">
      <AppMain />
    </div>
    <div class="buy-section-backgound">
      <AppBuySection />
    </div>
  </main>
  <footer>
    <div class="footer-backgound">
      <AppFooter />
    </div>
    <div class="sub-footer-backgound">
      <AppSubFooter />
    </div>
  </footer>
</template>

<style lang="scss">
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/variables' as *;

.main-jumbotron {
  background-image: url(../src/assets/img/jumbotron.jpg);
  background-size: cover;
  min-height: 400px;
}
.main-backgound {
  background-color: $dark-light;
}
.buy-section-backgound {
  background-color: $blue;
}
.footer-backgound {
  background-image: url(../src/assets/img/footer-bg.jpg);
  background-size: cover;
}
.sub-footer-backgound {
  background-color: $grey;
}
</style>