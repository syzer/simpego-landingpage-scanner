<template>
  <div>
    <Header />
    <main class="main" role="main">
      <nuxt/>
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">

html {
  font-family: $family-sans-serif;
  font-size: $body-size;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
}

*, *:before, *:after
{
  box-sizing: border-box;
  margin: 0;
}

body {
  background-color: $body-background-color;
  color: $text;
  font-size: 1rem;
  font-weight: 400;
  line-height: $body-line-height;
}

a {
  color: $link;
  text-decoration: none;
}

ul {
  padding: 0;
  list-style-type: none;
}

h1,
h2,
h3 {
  line-height: 1.15;
}

.main {
  margin-top: $header-height;
  min-height: calc(80vh);
}

.container {
  margin: 0 auto;
  position: relative;
  max-width: $maxPageWidth;
}

</style>
