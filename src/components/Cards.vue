<template>
  <div class="container">
    <h1 class="text-center m-3">Rick & Morty</h1>
    <div class="row">
      <div class="col-md-4 col-sm-12 carta-center" v-for="(item, index) in personajes" :key="index">
        <b-card :title="personajes[index].nombre" :img-src="personajes[index].imagen" img-alt="Image" img-top tag="article" style="max-width: 20rem;" class="mb-2">
        </b-card>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'Cards',
  data() {
    return {
      personajes: [
        {
          'id' : 1 ,
          'nombre' : 'Morty' ,
          'imagen' :
          'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
        },
        {
          'id' : 2 ,
          'nombre' : 'Rick' ,
          'imagen' :
          'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
        },
        {
          'id' : 3 ,
          'nombre' : 'Summer' ,
          'imagen' :
          'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
        },
        {
          'id' : 4 ,
          'nombre' : 'Beth' ,
          'imagen' :
          'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
        },
        {
          'id' : 5 ,
          'nombre' : 'Jerry' ,
          'imagen' :
          'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
        }
      ]
    }
  },
}
</script>

<style scoped>
  .carta-center{
    text-align: -webkit-center;
  }
</style>
