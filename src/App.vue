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
  <AppHeader />
  <AppMain />
  <AppBuySection />
  <AppFooter />
  <AppSubFooter />
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

</style>
