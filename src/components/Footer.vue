<template>
  <div class="contenitore">
    <div class="row">
      <div class="col_left">
        <ul>
          dc comics
          <li>
            <a href="#"></a>
          </li>
        </ul>
      </div>
      <div class="col_right">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      arrayFooter: [
        {
          text: 'Character'          
      }
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.row {
  height: 360px;
  background-image: url(../assets/img/footer-bg.jpg);
  display: flex;
  justify-content: space-around;
  overflow: hidden;
}
img {
  object-fit: contain;
  height: 110%;
}
</style>