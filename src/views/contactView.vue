<template>
  <body>
      <div class="contact_form">
          <div class="formulario">
            <h1 class="tituloo">¡Conversa conmigo!</h1>
            <h3>Tel: 3209759310 <br/> Pensilvania Caldas <br> aleja34n@gmail.com</h3>
            <form action="submeter-formulario.php" method="post">
            <p>
                <label for="nombre" class="colocar_nombre">Nombre
                <span class="obligatorio">*</span>
                <input type="text" name="introducir_nombre"
                id="nombre" required="obligatorio" placeholder="Escribe tu nombre"></label>
            </p>
            <p>
                <label for="email" class="colocar_email">Email
                <span class="obligatorio">*</span>
                <input type="email" name="introducir_email"
                id="email" required="obligatorio" placeholder="Escribe tu Email"></label>
            </p>
            <p>
                <label for="telefone" class="colocar_telefono">Telefono
                <input type="tel" name="introducir_telefono"
                id="telefono" placeholder="Escribe tu teléfono">
                </label>
            </p>
            <p>
                <label for="mensaje" class="colocar_mensaje">Mensaje
                <span class="obligatorio">*</span>
                <textarea name="introducir_mensaje" class="texto_mensaje"
                id="mensaje" required="obligatorio"
                placeholder="Deja aquí tu comentario..."></textarea>
                </label>
            </p>
            <div class="boton">
              <button type="submit" name="enviar_formulario" id="enviar"><p>Enviar</p></button>
            </div>
            <p class="aviso">
                 <span class="obligatorio"> * </span>Los campos son obligatorios
            </p>
           </form>
           </div>
         </div>
  </body>
</template>

<style>
.contact_form {
  margin: auto;
  margin-top: 8%;
  margin-bottom: 8%;
  width: 500px;
  height: auto;
  border-radius: 10px;
  padding-top: 30px;
  padding-bottom: 20px;
  padding-left: 30px;
  padding-right: 30px;
  background-color: #C4737C9E;
}

input {
  background-color: #fbfbfb;
  width: 408px;
  height: 40px;
  border-radius: 5px;
  border-style: solid;
  border-width: 1px;
  border-color: #C4737C9E;
  margin-top: 10px;
  padding-left: 10px;
  margin-bottom: 20px;
}

textarea {
  background-color: #fbfbfb;
  width: 405px;
  height: 150px;
  border-radius: 5px;
  border-style: solid;
  border-width: 1px;
  border-color: #ebc9bb;
  margin-top: 10px;
  padding-left: 10px;
  margin-bottom: 20px;
  padding-top: 15px;
}

label {
  display: block;
}

button {
  height: 45px;
  margin-bottom: 20px;
  margin-top: 10px;
  text-transform: uppercase;
  background-color: #C4737C9E;
  border-color: #C4737C9E;
  border-style: solid;
  border-radius: 10px;
  width: 420px;
  cursor: pointer;
  justify-content: flex-end;
}
button p {
  color: #fff;
}

span {
  color: #ebc9bb;
}

.aviso {
  color: #0e0e0e;
}

.tituloo {
  font-size: 39px;
  text-align: center;
  padding-bottom: 20px;
  color: #000000;
}

h3 {
  padding-bottom: 30px;
  color: #0e0e0e;
  text-align: center;
}

p {
  color: #0e0e0e;
  text-align: center;
}

::-webkit-input-placeholder {
  color: #a8a8a8;
}

::-webkit-textarea-placeholder {
  color: #a8a8a8;
}

.formulario input:focus {
  outline: 0;
  border: 1px solid #97d848;
}

.formulario textarea:focus {
  outline: 0;
  border: 1px solid #97d848;
}
</style>
