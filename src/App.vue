// Parte "HTML" dove posso "iniettare i miei componenti utilizzando "<component/>"

<template>
  <div id="app">
    <Title/>
    <Jumbotron/>
    
  </div>
</template>

// Parte Js dove importo i components.vue 

<script>
import Title from './components/Title.vue'
import Jumbotron from './components/Jumbotron.vue'

// qui esporto i componenti caricati in precedenza e li collego con id="app"

export default {
  name: 'app',
  components: {
    Title,
    Jumbotron
  }
}
</script>

parte CSS principale, le altri parti CSS vengono eseguite nei singoli componenti
<style lang="scss">

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    height: 100vh;
  }


</style>
