<template>
  <div class="about">
    <h1>Cualquier cosa ponemos aca</h1>
    <img src="../assets/logo.png">
    <hr>
    <p>{{ texto }}</p>
    <p id="parrafoDespedida">{{ despedida }}</p>
    <input type="text" v-bind:value="contenidoTexto"><br><br>
    <button v-on:click="despedirse" id="btnDespedida">Ver despedida</button>
  </div>
</template>
<script>
//creamos la etiqueta de script
//se debe exportar x defecto el modelo de datos
  export default{
    //llamada about-component
    name: 'about-component',
    data: function(){
      return{
        mensaje : 'Hola Mundo con VueJs',
        texto: 'Esto es un texto ',
        despedida: '',
        contenidoTexto: 'Contenido del modelo',
      }
    },
    methods:{
      despedirse : function(){
        this.despedida = 'Ya me voy mañana sigo estudiando'
      }
    }
  }
</script>
<style>
#btnDespedida{
  background-color: blueviolet;
}
#parrafoDespedida{
  background-color: chartreuse;
  color: black;
  font-size: 40px;
}
</style>
