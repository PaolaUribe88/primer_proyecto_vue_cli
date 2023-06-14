<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Mi personaje favorito de la saga de Harry Potter es Harry<br>
      podemos encontar su historia aqui
      <a href="https://es.wikipedia.org/wiki/Harry_Potter_(serie_cinematogr%C3%A1fica)" target="_blank" rel="noopener">Documentacion Harry Potter</a>.
    </p>
    <h3>Instale un Cli de Vue</h3>
    <ul>
      <li><img src="../assets/descarga.jpg"></li>
      <li><img src="../assets/dos.jpg"></li>
    </ul>
    <h3>Personajes Importantes</h3>
    <ul>
      <li><a href="https://harrypotter.fandom.com/es/wiki/Harry_Potter" target="_blank" rel="noopener">Harry Potter</a></li>
      <li><a href="https://www.fotogramas.es/noticias-cine/a17057795/que-tienes-de-ron-weasley/" target="_blank" rel="noopener">Ron Weasley</a></li>
      <li><a href="https://harrypotter.fandom.com/es/wiki/Hermione_Granger," target="_blank" rel="noopener">Hermaine Granger</a></li>
      <li><a href="https://harrypotter.fandom.com/es/wiki/Ginevra_Weasley" target="_blank" rel="noopener">Ginerva Weasley</a></li>
      <li><a href="https://harrypotter.fandom.com/es/wiki/Draco_Malfoy" target="_blank" rel="noopener">Draco Malfoyd</a></li>
    </ul>
    <h3>Listado de Peliculas</h3>
    <ul>
      <li><a href="https://es.wikipedia.org/wiki/Harry_Potter_y_la_piedra_filosofal_(pel%C3%ADcula)" target="_blank" rel="noopener">Harry Potter y la piedra filosofal </a></li>
      <li><a href="https://es.wikipedia.org/wiki/Harry_Potter_y_la_c%C3%A1mara_secreta_(pel%C3%ADcula)" target="_blank" rel="noopener">Harry Potter y la cámara secreta</a></li>
      <li><a href="https://en.wikipedia.org/wiki/Harry_Potter_and_the_Prisoner_of_Azkaban_(film)" target="_blank" rel="noopener">Harry Potter y el prisionero de Azkaban</a></li>
      <li><a href="https://es.wikipedia.org/wiki/Harry_Potter_y_el_c%C3%A1liz_de_fuego_(pel%C3%ADcula)" target="_blank" rel="noopener">Harry Potter y el cáliz de fuego</a></li>
      <li><a href="https://es.wikipedia.org/wiki/Harry_Potter_y_la_Orden_del_F%C3%A9nix_(pel%C3%ADcula)" target="_blank" rel="noopener">Harry Potter y la orden del Fénix</a></li>
      <li><a href="https://es.wikipedia.org/wiki/Harry_Potter_y_el_misterio_del_pr%C3%ADncipe_(pel%C3%ADcula)" target="_blank" rel="noopener">Harry Potter y el misterio del príncipe</a></li>
      <li><a href="https://en.wikipedia.org/wiki/Harry_Potter_and_the_Deathly_Hallows_%E2%80%93_Part_1" target="_blank" rel="noopener">Harry Potter y las reliquias de la muerte - Parte1</a></li>
      <li><a href="https://es.wikipedia.org/wiki/Harry_Potter_y_las_reliquias_de_la_Muerte:_parte_2" target="_blank" rel="noopener">Harry Potter y las reliquias de la muerte - Parte2</a></li>
      
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" agregue la palabra a scoped para limitar solo a este componente-->
<style scoped>
.hello{
  background-color: rgb(144, 177, 242);
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #51379b;
}
</style>
