<script>
import AppHeader from './components/header/AppHeader.vue';
import FooterNavbar from './components/footer/FooterNavbar.vue';
import FooterSocialLinks from './components/footer/FooterSocialLinks.vue';



export default {
  components: {
    AppHeader,
    FooterNavbar,
    FooterSocialLinks,
  }
}
</script>

<template>
  <AppHeader />
  <footer>
    <FooterNavbar />
    <FooterSocialLinks />
  </footer>
</template>

<style scoped lang="scss">

</style>
