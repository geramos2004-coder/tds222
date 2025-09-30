<template>
  <h1>Formulario : Gerardo Ramos</h1>


  <div class="form-container">
    <div>
      <label for="nombre">Nombre:</label>
      <input type="text" id="nombre" name="nombre" placeholder="Tu nombre" required>

      <label for="apellido">Apellido:</label>

      <input type="text" id="apellido" name="apellido" placeholder="Tu apellido" required>
    </div>

    <fieldset>
      <legend>Género:</legend>
      <label>

        <input type="radio" id="femenino" name="genero" value="femenino">
        Femenino
      </label>
      <label>
        <input type="radio" id="masculino" name="genero" value="masculino">
        Masculino
      </label>
    </fieldset>

    <div>
      <label for="fechaNacimiento">Fecha de Nacimiento:</label>
      <input type="date" id="fechaNacimiento" name="fechaNacimiento" required>

    </div>

    <div>
      <label for="email">Correo Electrónico:</label>
      <input type="email" id="email" name="email" placeholder="ejemplo@gmail.com" required>

    </div>

    <div>
      <label for="telefono">Teléfono:</label>
      <input type="tel" id="telefono" name="telefono" placeholder="123456789" pattern="[0-9]{8,15}">
      
    </div>

    <fieldset class="address-group">
      <legend>Dirección</legend>

      <div class="field-group">
        <div class="street-field">
          <label for="calle">Calle:</label>
          <input type="text" id="calle" name="calle" placeholder="Calle Principal #123" required>
        </div>
        <div class="colonia-field">
          <label for="colonia">Colonia:</label>
          <input type="text" id="colonia" name="colonia" required>
        </div>
      </div>

      <div class="field-group">
        <div>
          <label for="ciudad">Municipio:</label>
          <input type="text" id="ciudad" name="ciudad" required>
        </div>
        <div>
          <label for="estado">Departamento:</label>
          <input type="text" id="estado" name="estado" required>
        </div>
        <div>
          <label for="zip">Código Postal:</label>
          <input type="text" id="zip" name="zip" required>
        </div>
      </div>
    </fieldset>

    <div>
      <label for="mensaje">Mensaje:</label>
      <textarea id="mensaje" name="mensaje" rows="5" placeholder="Escribe tu mensaje aquí..." required></textarea>
    </div>

    <button type="submit" class="btn">Enviar</button>
  </div>
</template>

<script>
export default {
  name: "Formulario"
}
</script>

<style>
/* Contenedor principal */
.form-container {
  max-width: 650px;
  margin: auto;
  padding: 25px;
  background: #ffffff;
  border-radius: 16px;
  box-shadow: 0px 6px 20px rgba(0,0,0,0.1);
  font-family: "Segoe UI", Tahoma, sans-serif;
  color: #333;
}

/* Título */
h1 {
  text-align: center;
  margin-bottom: 20px;
  color: #2c3e50;
  font-size: 28px;
}

/* Etiquetas */
label {
  display: block;
  margin-bottom: 6px;
  font-weight: 600;
  color: #2c3e50;
}

/* Inputs y textarea */
input, textarea {
  width: 100%;
  padding: 12px;
  margin-bottom: 18px;
  border: 1.5px solid #d0d7de;
  border-radius: 8px;
  font-size: 15px;
  transition: all 0.3s ease;
  background-color: #f9fbfd;
}

input:focus, textarea:focus {
  border-color: #3db9a2;
  outline: none;
  background-color: #fff;
  box-shadow: 0 0 6px rgba(61, 185, 162, 0.3);
}

/* Fieldset */
fieldset {
  border: 1.5px solid #d0d7de;
  border-radius: 10px;
  margin-bottom: 20px;
  padding: 15px;
  background: #fefefe;
}

legend {
  font-weight: bold;
  padding: 0 10px;
  color: #3db9a2;
}

/* Grupos de campos */
.field-group {
  display: flex;
  gap: 15px;
  margin-bottom: 10px;
}

.field-group div {
  flex: 1;
}

/* Radio buttons */
fieldset label {
  display: inline-flex;
  align-items: center;
  margin-right: 20px;
  font-weight: normal;
  cursor: pointer;
}

input[type="radio"] {
  margin-right: 6px;
  accent-color: #3db9a2;
}

/* Botón */
.btn {
  background: linear-gradient(135deg, #42b983, #3db9a2);
  color: #fff;
  border: none;
  padding: 14px 20px;
  font-size: 16px;
  font-weight: bold;
  border-radius: 10px;
  cursor: pointer;
  width: 100%;
  transition: transform 0.2s ease, background 0.3s ease;
}

.btn:hover {
  transform: scale(1.02);
  background: linear-gradient(135deg, #3aa67f, #329c8a);
}
</style>
