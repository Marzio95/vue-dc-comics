<template>
  <div class="contenitore">
    <div class="jumbo">
      <div class="current">CURRENT SERIES</div>
    </div>
    <div class="row">
      <div class="container2">
        <CardDC
          v-for="element in arrayCard"
          :key="element.series"
          :card-src="element.thumb"
          :card-text="element.series"
        >
        </CardDC>
        <div class="center"><button class="load">LOAD MORE</button></div>
      </div>
    </div>
    <div class="row_blue">
      <div class="container">
        <ul>
          <li v-for="(element, index) in arrayMainbar" :key="index">
            <img :src="require('../assets/img/' + element.img)" alt="" />
            <a href="#">{{ element.text.toUpperCase() }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import CardDC from "./CardDC.vue";

export default {
  name: "MainDC",
  data() {
    return {
      arrayMainbar: [
        {
          img: "buy-comics-digital-comics.png",
          text: "digital comics",
        },
        {
          img: "buy-comics-merchandise.png",
          text: "dc merchandise ",
        },
        {
          img: "buy-comics-shop-locator.png",
          text: "subscription ",
        },
        {
          img: "buy-comics-subscriptions.png",
          text: "comic shop locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          text: "dc power visa",
        },
      ],
      arrayCard: [
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
  components: {
    CardDC,
  },
};
</script>

<style scoped lang="scss">
.jumbo {
  height: 400px;
  background-image: url(../assets/img/jumbotron.jpg);
  background-position-x: center;
  position: relative;
}
.current {
  background-color: #0282f9;
  width: 12rem;
  height: 2.5rem;
  line-height: 2.5rem;
  color: white;
  text-align: center;
  font-weight: 800;
  position: absolute;
  bottom: -1.25rem;
  left: 5rem;
}
.row {
  background-color: black;
  color: white;
  font-weight: 600;
  font-size: medium;
}
.row_blue {
  height: 120px;
  background-color: #0282f9;
  color: white;
  display: flex;
  justify-content: center;
}
.container {
  margin: auto;
  height: 100%;
  display: flex;
  align-items: center;
}
.container2 {
  width: 80%;
  margin: auto;
  display: flex;
  flex-wrap: wrap;
  padding: 3rem 0;
  gap: 1rem;
}
ul {
  display: flex;
  list-style: none;
}
li {
  display: flex;
  align-items: center;
  padding: 1rem;
  a {
    text-decoration: none;
    color: white;
    font-weight: bold;
    padding-left: 10px;
    font-size: 0.8rem;
  }
}
img {
  width: 50px;
  height: 50px;
  object-fit: contain;
}
.center {
  text-align: center;
  width: 100%;
}
.load {
  background: #0282f9;
  border: none;
  color: white;
  height: 3rem;
  width: 10rem;
  font-size: 1.2rem;
  font-weight: 700;
  cursor: pointer;
  margin-top: 1rem;
}
</style>
