<template>
  <div class="contenitore">
    <div class="row">
      <div class="container2">Content goes here</div>
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
    };
  },
};
</script>

<style scoped lang="scss">
.row {
  height: 120px;
  display: flex;
  align-items: center;
  background-color: black;
  color: white;
  font-weight: bold;
  font-size: 1.5rem;
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
</style>
