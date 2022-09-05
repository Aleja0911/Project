<template>
  <footer class="foot">
      <section >
         <div>
             <img class="img-footer" src="../assets/media/logo3.png" alt="logo">
         </div>
         <div>
             <h3>"La palabra como medicina" <br/>-MM</h3>
         </div>
       </section>
       <section class="redes">
         <div>
             <a href="https://www.instagram.com/alejaandra._11/">|<iconify-icon icon="logos:instagram-icon"></iconify-icon></a>
         </div>
         <div>
             <a href="https://github.com/Aleja0911">|<iconify-icon icon="icon-park:github"></iconify-icon></a>
         </div>
      </section>
      <small>&copy; 2022 <b> Aleja0911 </b></small>
  </footer>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'footerComp',
});
</script>

<style lang="scss">
.foot{
    text-align: center;
}
.img-footer{
    width: 15%;
    height: 15%;
}
.redes{
    display: flex;
    justify-content: center;
    padding: 3%;
}
</style>
