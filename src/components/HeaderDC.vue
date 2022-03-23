<template>
  <div class="container">
    <img src="../assets/img/dc-logo.png" alt="" />
    <ul>
      <li v-for="(element, index) in arrayNavbar" :key="index">
        <a href="#">{{ element.text.toUpperCase() }}</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HeaderDC",
  data() {
    return {
      arrayNavbar: [
        {
          text: "characters",
        },
        {
          text: "comics",
        },
        {
          text: "movies",
        },
        {
          text: "tv",
        },
        {
          text: "games",
        },
        {
          text: "collectibles",
        },
        {
          text: "videos",
        },
        {
          text: "fan",
        },
        {
          text: "news",
        },
        {
          text: "characters",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  width: 80%;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
li {
  display: inline-block;
  padding: 47px 1rem;
  height: 100%;
  border-bottom: 7px solid transparent;

  &:hover {
    border-bottom: 7px solid #0282f9;
  }
  &:hover a {
    color: #0282f9;
  }
  a {
    text-decoration: none;
    font-weight: bold;
  }
}
</style>
