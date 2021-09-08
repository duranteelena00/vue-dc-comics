<template>
  <main>
    <section id="products">
      <div class="container">
        <button>CURRENT SERIES</button>
        <ul>
          <li v-for="(item, index) in items" :key="index">
          <img :src="item.thumb">
          <p>{{item.series}}</p>
        </li>
        </ul>
        <button>LOAD MORE</button>
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
  data() {
    return {
      items: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<style scoped>
section#products {
  background: #202020;
  padding: 15px 0 20px 0;
}
  #products .container {
    position: relative;
     display: flex;
  flex-direction: column;
  }

#products .container,
#products ul {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
}

  #links ul {
    display: flex;
    justify-content: center;
    align-items: center;
    vertical-align: top;
  }

  #products li {
    flex-basis: calc(100% / 6.5);
    padding: 15px 0;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }

  #products li img {
    width: 100%;
    height: calc(900px / 6.5);
    object-fit: cover;
    object-position: top;
  }

  #products li p {
    padding-top: 10px;
    font-size: 11px;
    color: white;
    text-transform: uppercase;
  }

  #products button {
    padding: 7.5px 12.5px;
    background-color: #0c7cec;
    color: white;
    border: none;
    font-weight: bold;
  }

  #products button:first-of-type {
    position: absolute;
    top: -30px;
    left: 0;
    font-size: 14px;
  }

  #products button:nth-of-type(2) {
    margin-top: 10px;
    padding: 5px 30px;
    font-size: 10px;
    align-self: center;
  }

section#links {
  background: dodgerblue;
  padding: 40px 0;
  position: relative;
  z-index: 2;
}

#links .container {
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