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
    <div class="main-backgound">
      <AppMain />
    </div>
    <div class="buy-section-backgound">
      <AppBuySection />
    </div>
  </main>
  <div class="footer-backgound">
    <div class="container">
      <AppFooter />
    </div>
  </div>
  <div class="sub-footer-backgound">
    <div class="container">
      <AppSubFooter />
    </div>
  </div>
</template>

<style lang="scss">
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/variables' as *;

.main-backgound {
  background-color: $dark-light;
}

.buy-section-backgound {
  background-color: $blue;
}
/*.footer-backgound {

}*/
.sub-footer-backgound {
  background-color: $grey;
}



</style>
