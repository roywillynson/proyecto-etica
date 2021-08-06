<template>
<div>
  <header class="header hero is-fullheight-with-navbar pt-6">

    <video class="video is-absolute " :style="{ 'z-index': -1 }" src="~/assets/robot-bg.mp4" autoplay muted
      loop></video>

    <div class="hero-body mx-auto">

      <h1 class="title is-size-1 is has-text-centered has-text-warning p-6">
        Inteligencia Artificial
      </h1>
    </div>
  </header>

  <section class="section is-medium has-background-white" id="what-is">

    <div class="container columns px-6 is-flex is-justify-content-center is-align-items-center">

      <div class="column is-5 is-fullheigth is-overflow-hidden  has-text-centered">
        <img src="~/assets/ai.svg" alt="Inteligencia Artificial" :style="{ height: '300px' }">
      </div>

      <div class="column is-7">

        <h2 class="title is-size-2 has-text-black-ter pb-2">
          Inteligencia Artificial
        </h2>
        <p class="is-size-5">
          Se refiere a la simulación de la inteligencia humana en
          máquinas que están
          programadas para pensar como humanos e imitar sus acciones. El término también se puede aplicar a cualquier
          máquina que exhiba rasgos asociados con una mente humana, como el aprendizaje y la resolución de problemas.
        </p>
      </div>

    </div>
  </section>

  <section class="section is-medium has-background-warning-light" id="important">

    <div class="mb-6">
      <h2 class="title is-size-2 has-text-black-ter pb-2 has-text-centered">
        Importancia de la Inteligencia Artificial
      </h2>
      <h3 class="subtitle font-body has-text-centered has-text-grey">
        Aqui veremos porque es importante la inteligencia de la artificial
      </h3>
    </div>

    <div class="container columns is-multiline is-4 px-6 mx-0">

      <div class="column is-4" v-for="card in cards" :key="card.url">
        <Card :text="card.text" :url="card.url"/>
      </div>

    </div>
  </section>


  <section class="section is-medium has-background-white" id="impacto">

    <div class="container columns px-6">

      <div class="column is-5 is-fullheigth is-overflow-hidden  has-text-centered">
        <img src="~/assets/robot.jpg" alt="Robot de inteligencia artificial" :style="{ height: '100%', 'object-fit': 'cover' }">
      </div>

      <div class=" ml-6 column is-7">

        <h2 class="title is-size-2 has-text-black-ter pb-2">
          Impacto De La Inteligencia Artificial En La Vida De Las Personas
        </h2>
        <p class="is-size-5">
          La inteligencia artificial cada vez está más incrustada en nuestra sociedad y es más común entre nosotros,
          esta se encuentra en nuestros dispositivos, en nuestros trabajos, nuestra vida social y en las calles,
          automatizando tareas que realizan los humanos, aumentando la seguridad de nuestro dia a dia, muchas veces
          estos se encuentran decidiendo por nosotros como en los casos de los coches autónomos y/o asistiendo nos como
          en los casos de alexa, siri, entre otros asistentes virtuales.
          <br><br>
          En el futuro la inteligencia artificial superará las capacidades del ser humano y muchas personas quedarán sin
          trabajo aunque la vida será más fácil para ese futuro y esta nos permitirá un mayor tiempo para pensar en
          otros problemas de la humanidad y dedicar tiempo a lo que nos gusta.
        </p>
      </div>

    </div>
  </section>
</div>


</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'HomePage',
  data () {
    return {
      cards: [
        {
          text: 'La inteligencia artificial automatiza el aprendizaje y descubrimiento repetitivos a través de datos',
          url: require('~/assets/automatizacion.svg')
        },

        {
          text: 'IA agrega inteligencia a productos existentes.',
          url: require('~/assets/producto.svg')
        },
        {
          text: 'La inteligencia artificial se adapta a través de algoritmos de aprendizaje progresivo para permitir que los datos realicen la programación',
          url: require('~/assets/aprendizaje.svg')
        },

        {
          text: 'La inteligencia artificial analiza más datos y datos más profundos empleando redes neuronales que tienen muchas capas ocultas',
          url: require('~/assets/redes.svg')
        },
      ]
    }
  },
  components: {
    Card
  }
}
</script>

<style lang="scss" scoped>

@import "~bulma/sass/utilities/_all";

.video {
  position: fixed;
  right: 0;
  bottom: 0;
  min-width: 100%;
  min-height: 100%;
}

.hero-body > .title {
  border: 4px solid $yellow;
}

.header {
  background-color: rgba(0, 0, 0, 0.7);
}
</style>
