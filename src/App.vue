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
    <AppMain />
    <AppBuySection />
    <AppFooter />
    <AppSubFooter />
  </div>
</template>

<style lang="scss">
@use '../src/styles/general.scss' as *;
@use '../src/styles/partials/variables' as *;



</style>
