<template>
  <header class="container">
    <img src="@/assets/img/dc-logo.png" alt="" />
    <nav>
      <ul>
        <li v-for="(link, index) in links" :key="index">
          <a :href="link.url" :class="{ active: link.current }">{{
            link.text
          }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<style scoped>
header {
  padding: 15px 0;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

header img {
  width: 55px;
  height: auto;
}

nav {
  display: inline-flex;
}

ul {
  display: flex;
}

ul > li > a {
  margin: 0 10px;
  padding: 30px 0;
  font-size: 10px;
  font-weight: bold;
  color: rgb(75, 75, 75);
  text-transform: uppercase;
}

ul > li > a.active {
  color: dodgerblue;
  border-bottom: 4px solid dodgerblue;
}
</style>