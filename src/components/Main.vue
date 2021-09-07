<template>
  <main>
    <div class="container">
      <ul>
        <li>
            <a href="#"><img src="@/assets/img/buy-comics-digital-comics.png" alt="" />
            <span>digital comics</span></a>
        </li>
        <li>
            <a href="#"><img src="@/assets/img/buy-comics-merchandise.png" alt="" />
            <span>dc merchandise</span></a>
        </li>
        <li>
          <a href="#"><img src="@/assets/img/buy-comics-shop-locator.png" alt="" />
            <span>subscription</span></a>
        </li>
        <li>
          <a href="#"><img src="@/assets/img/buy-comics-subscriptions.png" alt="" />
            <span>comic shop locator</span></a>
        </li>
        <li>
          <a href="#"><img src="@/assets/img/buy-dc-power-visa.svg" alt="" />
            <span>dc power visa</span></a>
        </li>
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style scoped>
main {
  background: dodgerblue;
  padding: 40px 0;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

ul {
  display: flex;
  justify-content: center;
  align-items: center;
}

ul > li {
  padding: 0 20px;
}

ul > li > a {
  font-size: 10px;
  color: white;
  text-transform: uppercase;
  display: flex;
  justify-content: center;
  align-items: center;
}

li img {
    width: auto;
    margin-right: 10px;
}

li img:not(li:nth-of-type(5) img) {
    height: 40px;
}

li:nth-of-type(5)  img {
    height: 25px;
}
</style>