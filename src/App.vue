<template>
  <div id="app">
    <Header />
    <Hero />
    <Main />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Hero from "@/components/Hero.vue";
import Main from "@/components/Main.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Main,
  },
};
</script>

<style lang="css">
/* Utilities */
.container {
  max-width: 900px;
  height: 100%;
  margin: 0 auto;
}
/* Generics */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, Helvetica, sans-serif;
}

ul {
  list-style-type: none;
}

a {
  text-decoration: none;
}
</style>
