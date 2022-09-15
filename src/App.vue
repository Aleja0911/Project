<template>
  <!-- <div :class="getTheme()"> -->
    <nav class="nav-bar">
      <img class="nav-logo" src="./assets/media/Logo1.png" alt="Logo">
      <router-link to="/">Home</router-link>
      <router-link to="biography">Biography</router-link>
      <router-link to="/novels">Novels</router-link>
      <router-link to="/contact">Contact</router-link>
    </nav>
    <router-view/>
    <!-- <JcSwich id="page-style" v-model="isDarkMode"
       label="Go to dark" labelOFF="Go to ligth" /> -->
    <footerComp />
  <!-- </div> -->
</template>

<script>
// import { ref } from 'vue';
import footerComp from './components/footerComp.vue';

export default {
  components: { footerComp },
};

// const isDarkMode = ref(false);

// function getTheme() {
//   return isDarkMode.value ? 'theme--dark' : 'theme--light';
// }
</script>

<style lang="scss">
@use "./assets/styles/main.scss";
.nav-bar {
  display: flex;
  padding: 10px 20px;
  justify-content: space-evenly;
  background-color: var(--color-background-1);
  width: 100%;
}
.nav-logo{
  width: 30px;
  height: 30px;
  object-position: left;
  align-items: flex-start;
}
a {
  font-weight: bold;
  color: var(--color-text-1);
  text-decoration: none;

  &.router-link-exact-active {
  color:#C4737C9E;
}
}
</style>
