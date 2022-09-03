<template>
    <nav class="nav-bar">
      <img class="nav-logo" src="./assets/media/Logo1.png" alt="Logo">
      <router-link to="/">Home</router-link> |
      <router-link to="/biography">biography</router-link> |
      <router-link to="/novels">novels</router-link> |
      <router-link to="/contact">contact</router-link>
    </nav>
    <router-view/>
</template>

<style lang="scss">
@use "./assets/styles/main.scss";
.nav-bar {
  display: flex;
  justify-content: space-between;
  padding: 10px 20px;
  background-color: aqua;
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

  &.router-link-exact-active {
      color: var(--color-click-navbar);
  }
}
</style>
