<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  name: 'App',
  components: {
    Header
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
  margin: 0 auto;
}

a {
  text-decoration: none;
}
</style>
