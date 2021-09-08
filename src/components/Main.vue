<template>
  <main>
    <section id="products">
      <div class="container">
        <ul>
          <li></li>
        </ul>
      </div>
    </section>
    <section id="links">
      <div class="container">
        <ul>
          <li>
            <a href="#"
              ><img src="@/assets/img/buy-comics-digital-comics.png" alt="" />
              <span>digital comics</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img src="@/assets/img/buy-comics-merchandise.png" alt="" />
              <span>dc merchandise</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img src="@/assets/img/buy-comics-shop-locator.png" alt="" />
              <span>subscription</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img src="@/assets/img/buy-comics-subscriptions.png" alt="" />
              <span>comic shop locator</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img src="@/assets/img/buy-dc-power-visa.svg" alt="" />
              <span>dc power visa</span></a
            >
          </li>
        </ul>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style scoped>
section#products {
  height: 350px;
  background: #202020;
}

  #products ul,
  #links ul {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
section#links {
  background: dodgerblue;
  padding: 40px 0;
  position: relative;
  z-index: 2;
}

section#links .container {
  display: flex;
  justify-content: center;
  align-items: center;
}

#links ul > li {
  padding: 0 20px;
}

#links ul > li > a {
  font-size: 10px;
  color: white;
  text-transform: uppercase;
  display: flex;
  justify-content: center;
  align-items: center;
}

#links li img {
  width: auto;
  margin-right: 10px;
}

#links li img:not(li:nth-of-type(5) img) {
  height: 40px;
}

#links li:nth-of-type(5) img {
  height: 25px;
}

</style>