<template>
  <footer>
    <section>
      <div class="container">
        <div class="lists">
          <ul>
            <li><h4>DC Comics</h4></li>
            <li><a href="#">Characters</a></li>
            <li><a href="#" class="active">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>

          <ul>
            <li><h4>DC</h4></li>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policy</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshop</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>

          <ul>
            <li><h4>Sites</h4></li>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>

          <ul>
            <li><h4>Shop</h4></li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <img src="@/assets/img/dc-logo-bg.png" alt="" />
      </div>
    </section>
    <section>
      <div class="container">
        <div>
          <button>SIGN-UP NOW!</button>
        </div>
        <ul>
          <li><h4>FOLLOW US</h4></li>
          <li>
            <a href="#"
              ><img src="@/assets/img/footer-facebook.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="@/assets/img/footer-periscope.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"
              ><img src="@/assets/img/footer-pinterest.png" alt=""
            /></a>
          </li>
          <li>
            <a href="#"><img src="@/assets/img/footer-twitter.png" alt="" /></a>
          </li>
          <li>
            <a href="#"><img src="@/assets/img/footer-youtube.png" alt="" /></a>
          </li>
        </ul>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
section:first-of-type {
  background-image: url("../assets/img/footer-bg.jpg");
  height: 250px;
}

.container {
  display: flex;
}

section:first-of-type > .container {
  justify-content: space-between;
}

.lists {
  padding: 30px 0 40px 0;
  display: flex;
}

section:first-of-type ul {
  margin-right: 30px;
}

section:first-of-type ul li h4 {
  margin-bottom: 10px;
  font-size: 13px;
  color: white;
  text-transform: uppercase;
}

section:first-of-type ul li:not(li:first-of-type) {
  line-height: 12px;
}

ul li a {
  font-size: 10px;
  color: grey;
}

section:first-of-type img {
  height: 380px;
  margin-top: -65px;
  z-index: 1;
}

section:nth-of-type(2) {
  height: 80px;
  background: #363636;
  position: relative;
  z-index: 2;
}

section:nth-of-type(2) > .container {
  justify-content: space-between;
  align-items: center;
}

section:nth-of-type(2) button {
  padding: 7.5px;
  border: 2px solid #0c7cec;
  background: transparent;
  font-size: 12px;
  color: white;
}

section:nth-of-type(2) ul {
  display: flex;
  align-items: center;
}

section:nth-of-type(2) ul h4 {
  margin-right: 15px;
  color: #0c7cec;
  font-size: 13px;
  font-weight: bold;
}

section:nth-of-type(2) ul > li > a {
  margin: 5px;
}

section:nth-of-type(2) ul > li > a > img {
  height: 25px;
  width: auto;
}
</style>