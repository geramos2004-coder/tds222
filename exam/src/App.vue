<template>
  <h1>Formulario</h1>

 <div>
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" placeholder="Tu nombre" required>
        
        <label for="apellido">Apellido:</label>
        <input type="text" id="apellido" name="apellido" placeholder="Tu apellido" required>
    </div>

     <fieldset>
        <legend>Género:</legend>
        
        <input type="radio" id="femenino" name="genero" value="femenino">
        <label for="femenino">Femenino</label>
        
        <input type="radio" id="masculino" name="genero" value="masculino">
        <label for="masculino">Masculino</label>
        
  
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
        <input type="tel" id="telefono" name="telefono" 
               placeholder=" 123456789" 
               pattern="[0-9]{8,15}">
    </div>


     <fieldset class="address-group">
        <legend>Dirección</legend>

        <div class="field-group">
            <div class="street-field">
                <label for="calle">Calle:</label>
                <input type="text" id="calle" name="calle" placeholder=" Calle Principal #123" required>
            </div>
            <div class="colonia-field">
                <label for="colonia">Colonia:</label>
                <input type="text" id="colonia" name="colonia" required>
            </div>
        </div>
        
        <div class="field-group">
            <div>
                <label for="ciudad">Municiopio:</label>
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
      <button type="submit">Enviar Registro</button>


</template>

<script>

</script>

<style>
/* Contenedor general */
.form-container {
  max-width: 600px;
  margin: auto;
  padding: 20px;
  background: #f7f9fc;
  border-radius: 12px;
  box-shadow: 0px 4px 10px rgba(0,0,0,0.1);
  font-family: Arial, sans-serif;
}

/* Título */
h1 {
  text-align: center;
  margin-bottom: 20px;
  color: #333;
}

/* Etiquetas */
label {
  display: block;
  margin-bottom: 6px;
  font-weight: bold;
  color: #444;
}

/* Inputs y textarea */
input, textarea {
  width: 100%;
  padding: 10px;
  margin-bottom: 15px;
  border: 1px solid #ccc;
  border-radius: 6px;
  font-size: 14px;
  transition: border 0.3s;
}

input:focus, textarea:focus {
  border-color: #42b983;
  outline: none;
  box-shadow: 0px 0px 5px rgba(66, 185, 131, 0.5);
}

/* Fieldset */
fieldset {
  border: 1px solid #ddd;
  border-radius: 8px;
  margin-bottom: 20px;
  padding: 15px;
  background: #fff;
}

legend {
  font-weight: bold;
  color: #333;
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

/* Botón */
.btn {
  background: #42b983;
  color: #fff;
  border: none;
  padding: 12px 20px;
  font-size: 16px;
  border-radius: 6px;
  cursor: pointer;
  width: 100%;
  transition: background 0.3s;
}

.btn:hover {
  background: #2a9d6f;
}
</style>
