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
    

</template>

<script>

</script>

<style>

</style>
