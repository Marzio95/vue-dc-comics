<template>
  <div class="card">
    <img :src="cardSrc" :alt="cardText" />
    <h3>{{ cardText }}</h3>
  </div>
</template>

<script>
export default {
  name: "CardDC",
  props: {
    cardSrc: String,
    cardText: String,
  },
};
</script>

<style scoped lang="scss">
.card {
  width: calc(100% / 6 - 1rem);
}
img {
  width: 100%;
}
h3 {
  color: white;
  font-size: medium;
  font-weight: 500;
  margin-top: 8px;
  text-transform: uppercase;
}
</style>
