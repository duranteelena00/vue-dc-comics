<template>
  <div id="app">
    <Header />
    <Hero />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Hero from "@/components/Hero.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Main,
    Footer,
  },
};
</script>

<style lang="css">
/* Utilities */
html {
  width: 100vw;
  height: 100vh;
}

body {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

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
