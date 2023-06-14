<template>
  <div class="home">
    <img alt="Vue logo" v-bind:src="imagenaMostrar" ><br>
    <button v-on:click="cargarHarry">Ver Harry</button>
    <button v-on:click="cargarMarty">Ver Marty</button>
    <HelloWorld msg="Bienvenido a Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    //este padre home le manda mensajes al componente hijo helloword
    HelloWorld
  },
  data: function(){
    return{
      imagenHarry: '../assets/img/harry.jpg',
      imagenMarty: '../assets/img/marty.jpg',
      imagenaMostrar: '',
      textoAMostrar:''
    }
  },
  methods: {
    cargarHarry: function(){
      this.imagenaMostrar = this.imagenHarry;
      this.textoAMostrar = 'Harry';

    },
    cargarMarty: function(){
      this.imagenaMostrar = this.imagenMarty;
      this.textoAMostrar = 'Marty'

    }
  }
}
</script>
<style scoped>

</style>