<template>
    <section class="phrases">
        <div class="item1">
          <h1 class="titlee">FRASES RELEVANTES</h1>
        </div>

        <div class="item2">
          <h3>“La creación es femenina, el caos es masculino”</h3>
        </div>

        <div class="item3">
            <h3>“La crueldad del olvido, tan necesaria para
                 sobrevivir.” <br/> ― Mario Mendoza, La
                 ciudad de los umbrales</h3>
        </div>

        <div class="item4">
            <h3>“Parece mentira, pero existimos para otros,
             somos lo que somos porque los demás nos sirven
             de espejo para definirnos” <br/> ― Mario Mendoza,
             Relato de un asesino</h3>
        </div>

        <div class="item5">
            <h3>“Ciudad gótica no da tregua. Sus murallas son
              una metáfora de nuestra propia incapacidad para
              superar nuestros límites, Estamos atrapados en
              nosotros mismos”. <br/> - Akelarre. </h3>
        </div>

        <div class="item6">
            <h3>“Deja atrás todo, no te aferres, libérate de
             la peor carga de todas: tú mismo.” <br/>― Mario
             Mendoza, Akelarre</h3>
        </div>

        <div class="item7">
            <h3>“Mira, la ciudad es enorme, gigantesca, y sin
             embargo nadie está penando en nosotros ahora,
             nadie nos extraña, a nadie le hacemos falta… qué
             vértigo”<br/>-Una escalera al cielo. </h3>
        </div>
    </section>
</template>
<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'phrasesComp',
});
</script>

<style lang="scss">
.item1{
    grid-area: c;
    margin: 6%;
    text-align: center;
    background-color: #C4737CE8;
    height: 50%;
    padding: 3%;

    .titlee{
        padding-top: 15px;
    }
}
.item2{
    grid-area: d;
    text-align: center;
    padding: 20%;
    margin: 5%;
    background-color: #C4737C9E;
}
.item3{
    grid-area: e;
    text-align: center;
    padding: 20%;
    margin: 5%;
    background-color: #C4737CE8;
}
.item4{
    grid-area: f;
    text-align: center;
    padding: 15%;
    margin: 5%;
    background-color: #C4737C9E;
}
.item5{
    grid-area: g;
    text-align: center;
    padding: 15%;
    margin: 5%;
    background-color: #C4737CE8;
}
.item6{
    grid-area: h;
    text-align: center;
    padding: 18%;
    margin: 5%;
    background-color: #C4737C9E;
}
.item7{
    grid-area: i;
    text-align: center;
    padding: 15%;
    margin: 5%;
    background-color: #C4737CE8;
}

.phrases{
  display: grid;
  grid-template-rows: auto auto;
  grid-template-areas:
  "c"
  "d"
  "e"
  "f"
  "g"
  "h"
  "i";
}

@media (min-width: 600px) {
    .phrases {
      grid-template-areas:
       "c  c  c"
       "d  e  f"
       "g  h  i";
    }
}
</style>
