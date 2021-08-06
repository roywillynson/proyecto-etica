<template>
  <div>
    <nav class="navbar is-fixed-top is-transparent" role="navigation" aria-label="main navigation">
      <div class="container">

        <div class="navbar-brand">
          <nuxt-link class="navbar-item" to="/">
            <p class="is-size-3 has-text-weight-bold" title="Inteligencia Artificial">IA</p>
          </nuxt-link>

          <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navMenu" class="navbar-menu">
          <div class="navbar-end">
            <a class="navbar-item" href="#what-is">
              <button class="button is-warning is-rounded">AI</button>
            </a>
            <a class="navbar-item" href="#important">
              <button class="button is-warning is-rounded">Importancia</button>
            </a>
            <a class="navbar-item" href="#impacto">
              <button class="button is-warning is-rounded">Impacto de la IA</button>
            </a>
          </div>

        </div>
      </div>
    </nav>

    <Nuxt />
  </div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&family=Rubik:wght@500;700&display=swap');

$font-title: 'Rubik', sans-serif;
$font-body: 'Roboto', sans-serif;

h1, h2, h3, h4, h5, h6 {
  font-family: $font-title;
  letter-spacing: 1px;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: $font-body;
}

.font-body {
  font-family: $font-body;
}

.font-title {
  font-family: $font-title;
}

</style>
