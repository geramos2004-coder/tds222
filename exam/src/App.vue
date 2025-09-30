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
    

</template>

<script>

</script>

<style>

</style>
