<template>
  <div class="contenitore">
    <div class="row">
      <div class="container">Content goes here</div>
    </div>
    <div class="row_blue">
      <div class="container">
        <ul>
          <li v-for="(element, index) in arrayMainbar" :key="index">
            <img :src="element.img" alt="" />
            <a href="#">{{ element.text.toUpperCase() }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Main",
  data() {
    return {
      arrayMainbar: [
        {
          img: '../assets/img/buy-comics-digital-comics.png',
          text: "digital comics",
        },
        {
          img: 'buy-comics-digital-comics.png',
          text: "digital comics",
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
}
.container {
  width: 80%;
  margin: auto;
  height: 100%;
  display: flex;
  align-items: center;
}
ul{
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
  }
}
img{
    width: 60px;
    height: 60px;
}
</style>