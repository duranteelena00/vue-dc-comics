<template>
  <div id="app">
    <Header/>
    <Hero/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Hero from '@/components/Hero.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero
  }
}
</script>

<style lang="css">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}

.container {
  max-width: 900px;
  height: 100%;
  margin: 0 auto;
}

a {
  text-decoration: none;
}
</style>
