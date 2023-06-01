<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
import AppMain from './components/AppMain.vue'

export default {
  components: {
    AppHeader,
    AppFooter,
    AppMain

  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/partials/variables.scss' as *;
@use './styles/general.scss' as *;
</style>
