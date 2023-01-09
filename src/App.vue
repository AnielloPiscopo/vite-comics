<script>
import AppHeader from './components/header/AppHeader.vue';
import MainContent from './components/main/MainContent.vue';
import MainNavbar from './components/main/MainNavbar.vue';
import FooterNavbar from './components/footer/FooterNavbar.vue';
import FooterSocialLinks from './components/footer/FooterSocialLinks.vue';



export default {
  components: {
    AppHeader,
    MainContent,
    MainNavbar,
    FooterNavbar,
    FooterSocialLinks,
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <MainContent />
    <MainNavbar />
  </main>
  <footer>
    <FooterNavbar />
    <FooterSocialLinks />
  </footer>
</template>

<style scoped lang="scss">

</style>
