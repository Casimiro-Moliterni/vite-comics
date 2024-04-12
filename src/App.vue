<script>
import AppHeader from './components/AppHeader.vue'
import AppCards from './components/AppCards.vue'
import AppCardsFontAwesome from './components/AppCardsFontAwesome.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components:{
    AppHeader,
    AppCards,
    AppCardsFontAwesome,
    AppFooter
  }
}
</script>

<template>
  <AppHeader></AppHeader>
  <main>
    <AppCards></AppCards>
    <AppCardsFontAwesome></AppCardsFontAwesome>
  </main>
  <footer>
    <AppFooter></AppFooter>
  </footer>
</template>

<style lang="scss">
@use './style/generic';
</style>