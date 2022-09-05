<template>
  <header class="home">
    <h1 class="title-home">"Leer es resistir" <br/>-MM </h1>
  </header>
  <body>
    <section class="description">
      <div class="item-1">
        <h1 class="info-title">CITY OF READERS</h1>
        <p class="info-subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit.
        Amet repellendus voluptas natus dicta praesentium.
        Laboriosam nesciunt, incidunt quaerat iste eligendi repudiandae optio
        repellendus, harum labore aliquid,
        laudantium quis ratione eos?</p>
      </div>
      <div class="item-2">
        <img class="logo-img" src="../assets/media/Logo2.png" alt="Logo del sitio">
      </div>
    </section>
    <PhrasesComp />
  </body>
</template>

<script>
import PhrasesComp from '@/components/phrasesComp.vue';
// @ is an alias to /src
export default {
  name: 'HomeView',
  components: { PhrasesComp },
};
</script>
<style lang="scss">
/* home */
.home{
  background: url(../assets/media/portadaa.png);
  width: 100%;
  height: 450px;
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
.title-home{
  text-align: center;
  padding-top: 10%;
  padding-bottom: 10%;
  font-size: 4rem;
  color: var(--color-text-home);
}
/* description */
.item-1{
  grid-area: a;
  text-align: center;
  margin: auto;
  padding: 15%;
}
.info-title{
  padding: 5%;
}
.item-2{
  grid-area: b;
  text-align: center;
  justify-content: center;
  margin: auto;
}
.logo-img{
  width: 40%;
  height: 40%;
}
.description{
  display: grid;
  grid-template-columns: repeat(2,1fr);
  grid-template-rows: auto auto;
  grid-template-areas:
   "a  a"
   "b  b";
}
@media (min-width: 600px) {
  .description {
    grid-template-areas:
    "a b";
  }
}
</style>
