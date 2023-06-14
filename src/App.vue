<template>
  <div id="app">
    <nav>
      <router-link to="/">Inicio</router-link> |
      <router-link to="/about">Version</router-link>
    </nav>
    <router-view/> 
    <hr>
      <div class="prueba">
        <p>Contenido</p>
        <p id="parrafoMsje">{{ mensaje }}</p>
        <p id="parrafoSaludo">{{ saludo }}</p>
        <button v-on:click="saludar">Ver Saludo</button>
      </div>
  </div>
 
</template>
<script>
//creamos la etiqueta de script
//se debe exportar x defecto el modelo de datos
  export default{
    //llamada app-component
    name: 'app-component',
    data: function(){
      return{
        mensaje : 'Hola Mundo con VueJs',
        otromensaje: 'Estamos Trabajando con VueJs 2',
        saludo: ''
      }
    },
    methods:{
      saludar : function(){
        this.saludo = 'Estamos Cambiando una propiedad del modelo de datos'
      }
    }
  }
</script>

<style>
body{
  background-color:rgb(160, 251, 221);
}
.prueba{
  background-color: #10015b;
  color:yellowgreen;
}
#parrafoSaludo{
  color: white;
  font-size: 35px;
}
#parrafoMsje{
  font-size: 50px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #26096f;
}

nav {
  padding: 30px;
  
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #10015b;
}
</style>
