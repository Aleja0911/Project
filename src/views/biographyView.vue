<template>
  <body class="grid-container">
    <aside class="sidebar">
      <div>
        <img class="img-a" src="../assets/media/mario.jpg" alt="cucho mario">
      </div>
      <div class="textos">
        <h1 style="padding:5%;">Mario Mendoza Zambrano</h1>
        <h3>(Bogotá, 10 de Enero 1964)<br/>Escritor y periodista Colombiano.</h3>
      </div>
    </aside>
    <main class="main">
      <div>
        <h1 style="text-align: center;">Biografía</h1>
      </div>
      <article>
        <p>Mario Mendoza Zambrano nació en 1964 en Bogotá, Colombia. Estudió en la Pontificia
        Universidad Javeriana de
        Bogotá donde obtuvo la maestría en Literatura Latinoamericana. Luego de licenciarse en
        literatura y trabajar como
        pedagogo, Mendoza, decidió iniciar su carrera literaria a partir de 1980, combinando la
        escritura con la docencia y
        la colaboración con diversos medios culturales
        como diarios y revistas,entre esas, la Revista
        Bacánika. Ha
        impartido clases
        de literatura durante más
        de diez años.Su primera  novela,
        La ciudad de los umbrales, fue publicada
        en 1992. Tan sólo dos
        años más tarde
        fue galardonado con el Premio Nacional
        de Literatura de Colombia por La
        travesía del vidente.Gracias a su novela Satanás, Mario,obtuvo del Premio
        Biblioteca Breve de la editorial Seix
        Barral en 2002. Mendoza es uno de los más reconocidos autores
        latinoamericanos de la actualidad.
        </p>
       <h1 style="text-align: center;">PREMIOS</h1>
       <ul>
        <li>Premio Nacional de Literatura del Instituto
        Distrital de Cultura y Turismo de Bogotá (1995)</li>
        <li>Premio Biblioteca Breve de Seix Barral con la novela Satanás (2002)</li>
        <li>Premio Nacional de Literatura ~ Libros y Letras (2011)</li>
       </ul>
      </article>
    </main>
  </body>
</template>

<style lang="scss">
.sidebar{
  grid-area: a;
  background-color: #C4737CE8;
  margin: 2%;
  text-align: center;
}
.img-a{
  width: 90%;
  height: 100%;
  padding-top: 5%;
}
.textos{
  padding-top: 15%;
}
.main{
  grid-area: b;
  background-color:#C4737C9E;
  width: auto;
  padding: 5%;
  margin: 2%;
  text-align: justify;
}
.grid-container{
  font-size: 1.5rem;
  display: grid;
  grid-template:
  "a"
  "b";
}
@media (min-width: 600px) {
  .grid-container{
    grid-template:
    "a  b";
  }
  .sidebar{
    width: 200px;
    height: auto;
  }
  .main{
    width: auto;
    height: auto;
  }
}
@media (min-width: 900px) {
  .grid-container {
    grid-template:
    "a  b";
  }
  .sidebar{
    width: 300px;
    height: auto;
  }
  .main{
    width: auto;
    height: auto;
  }
}
</style>
