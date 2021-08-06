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
        Importancia de la Inteligencía Artificial
      </h2>
      <h3 class="subtitle font-body has-text-centered has-text-grey">
        Aqui veremos porque es importante la inteligencía de la artificial
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
          Impacto De La Inteligencía Artificial En La Vida De Las Personas
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

  <section class="section is-medium has-background-warning-light" id="important">

    <div class="mb-6">
      <h2 class="title is-size-2 has-text-black-ter pb-2 has-text-centered">
        Ventajas y Desventajas de la IA
      </h2>
    </div>

    <div class="container columns is-multiline is-4 px-6 mx-0 is-size-5">


      <h3 class="mb-4">Las ventajas son:</h3>
      <div class="mb-6">
        <div class="notification p-4">
          Es disminuir la muerte en trabajos riesgosos reemplazando al humano.
        </div>

        <div class="notification p-4">
          Mayor precisión a la hora de detectar enfermedades o patrones, sabemos que las máquinas pueden procesar
          millones
          de datos por segundos, en el futuro los médicos podrían solo dedicarse a aplicar medicamentos y puede que
          existan
          máquinas que detectan una enfermedad con una radiografía con un margen de error menor al humano, esto traerá
          ventajas a la medicina y la humanidad.
        </div>

        <div class="notification p-4">
          Disminuir la delincuencia, debido a la sobrevigilancia.
        </div>
      </div>



      <h3 class="mb-4">Las desventajas son:</h3>
      <div class="mb-6">
        <div class="notification p-4">
          La sobrevigilancia, la ia siempre está constantemente minando nuestros datos para poder funcionar
          correctamente,
          desde tu banda electrónica que marca tus pasos y presión cardiaca hasta las apps de tu celular que captan tu
          información para recomendarte contenido.
        </div>

        <div class="notification p-4">
          Aumento del desempleo, debido a que estas máquinas podrán realizar las mismas tareas que los seres humanos sin
          cansarse.
        </div>

        <div class="notification p-4">
          Costos y tiempos de implementación de la misma, muchos de estos proyectos requieren de una gran financiación,
          mucho tiempo para que puedan funcionar de forma eficiente y se necesita expertos cualificados.
        </div>
      </div>

    </div>
  </section>

  <section class="section is-medium has-background-white" id="impacto">

    <div class="container columns px-6">

      <div class="column is-7 mr-6">
        <h2 class="title is-size-2 has-text-black-ter pb-2">
          Moral y Etica en la Inteligencía Artificial
        </h2>
        <p class="is-size-5">
          La inteligencia artificial como podemos ver facilita nuestro día pero también provoca la sobrevigilancia y
          viola nuestra privacidad por eso hay que poner unas normas morales para detener estas cosas, ¿Que es más
          importante tu privacidad o seguridad? son cosas que se están debatiendo en la actualidad.
          <br><br>

          Hay dilemas morales a lo que nos enfrentamos respecto a la ia actualmente, un ejemplo: una persona va a chocar
          a otro persona, pero al lado solo hay una pared de concreto, que debe hacer la máquina, chocar a la persona
          delante y salvar al que va en el carro o chocar el concreto y salvar a la persona delante, hay otras
          cuestiones como cuántas personas iban en el carro o delante, muchos prefieren dejárselo al destino y no
          interferir y otros prefieren que la máquina decida por ellos. Como podemos ver las máquinas no siempre pueden
          decidir en nuestro dia a dia debido a la ética y moral, no siempre es correcto que la máquina intervenga en
          algunos procesos en lo que está puesto en una cuestión ética.

          <br><br>

          En conclusión, la inteligencia artificial a mejorado la vida del ser humano debido a la automatización de las
          laborales del ser humano volviéndose dependiente de esta, pero también tiene su lado oscuro con las empresas
          que nos espían y le regalamos nuestra privacidad a cambio de esta seguridad y comodidad en nuestro día a día,
          vemos como en procesos morales esta se encuentra limitada y por principios éticos no sabemos si es correcto
          que una máquina decida por nosotros, en situaciones de peligro ya que atenta contra nuestros principios éticos
          y los de los demás.Sin embargo límite de la inteligencia artificial y a lo que esta puede llegar será nuestra
          imaginación.

        </p>
      </div>

      <div class=" column is-5 is-fullheigth is-overflow-hidden  has-text-centered">

        <img src="~/assets/robot.jpg" alt="Robot de inteligencia artificial"
          :style="{ height: '100%', 'object-fit': 'cover' }">
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
