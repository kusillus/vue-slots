<template>
  <div id="app">
    <!-- Cuando mandamos data -->
    <card>
      <span slot="top">{{top}}</span>
      <h4 slot="title">{{title}}</h4>
      <p slot="body">{{description}}</p>
    </card>
    <!-- cuando no enviamos nada -->
    <card></card>
  </div>
</template>

<script>
import card from './components/cCard.vue'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      top: 'Pokemon',
      title: 'Pokemon Red',
      description: 'El nombre del protagonista puede ser escogido por el jugador, aunque su nombre genérico es Rojo. El Profesor Oak te permitirá elegir uno de entre tres Pokémon iniciales (Bulbasaur, Charmander y Squirtle) para iniciar la aventura y poder combatir contra otros Pokémon salvajes y entrenadores.'
    }
  },
  components: {
    card
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}
h4, p{
  margin: 0;
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
  color: #42b983;
}
</style>
