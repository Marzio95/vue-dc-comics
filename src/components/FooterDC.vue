<template>
  <div class="contenitore">
    <div class="row">
      <div class="col_left">
        <div>
          <ul>
            <h3>DC COMICS</h3>
            <li v-for="(element, index) in arrayFooter1" :key="index">
              <a href="#">{{ element.text }}</a>
            </li>
          </ul>

          <ul>
            <h3>SHOP</h3>
            <li v-for="(element, index) in arrayFooter2" :key="index">
              <a href="#">{{ element.text }}</a>
            </li>
          </ul>
        </div>

        <div>
          <ul>
            <h3>DC</h3>
            <li v-for="(element, index) in arrayFooter3" :key="index">
              <a href="#">{{ element.text }}</a>
            </li>
          </ul>
        </div>

        <div>
          <ul>
            <h3>SITES</h3>
            <li v-for="(element, index) in arrayFooter4" :key="index">
              <a href="#">{{ element.text }}</a>
            </li>
          </ul>
        </div>
      </div>

      <div class="col_right">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
    </div>
    <div class="edit">
      <div class="col_edit_left">
        <button>SIGN-UP NOW!</button>
      </div>

      <div class="col_edit_right">
        <div class="follow">FOLLOW US</div>
        <img src="../assets/img/footer-facebook.png" alt="" />
        <img src="../assets/img/footer-twitter.png" alt="" />
        <img src="../assets/img/footer-youtube.png" alt="" />
        <img src="../assets/img/footer-pinterest.png" alt="" />
        <img src="../assets/img/footer-periscope.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterDC",
  data() {
    return {
      arrayFooter1: [
        {
          text: "Character",
        },
        {
          text: "Comics",
        },
        {
          text: "Movies",
        },
        {
          text: "TV",
        },
        {
          text: "Games",
        },
        {
          text: "Videos",
        },
        {
          text: "News",
        },
      ],
      arrayFooter2: [
        {
          text: "Shop DC",
        },
        {
          text: "Shop DC Collectibles",
        },
      ],
      arrayFooter3: [
        {
          text: "Terms Of Use",
        },
        {
          text: "Privacy policy (News)",
        },
        {
          text: "Ad Choices",
        },
        {
          text: "Adversiting",
        },
        {
          text: "Jobs",
        },
        {
          text: "Subscriptions",
        },
        {
          text: "Talent Workshop",
        },
        {
          text: "CPSC Certificates",
        },
        {
          text: "Ratings",
        },
        {
          text: "Shop Help",
        },
        {
          text: "Contact Us",
        },
      ],
      arrayFooter4: [
        {
          text: "DC",
        },
        {
          text: "MAD Magazine",
        },
        {
          text: "DC Kids",
        },
        {
          text: "DC Universe",
        },
        {
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.row {
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  display: flex;
  justify-content: space-around;
  align-items: center;
  overflow: hidden;
}
img {
  object-fit: contain;
  height: 110%;
}
.col_left {
  display: flex;
}
ul {
  color: white;
  list-style: none;
  font: bold;
}
h3 {
  font-size: 1.5rem;
}
li {
  padding: 0.15rem;
}
a {
  text-decoration: none;
  color: gray;
  font-weight: bold;
}
.edit {
  background-color: #303030;
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 6rem;
}
.col_edit_right {
  display: flex;
  align-items: center;
}
img {
  padding: 0 0.4rem;
}
.follow {
  color: #0282f9;
  padding-right: 1.4rem;
  font-weight: bold;
  font-size: 1.4rem;
}
button {
  border: 2px solid #0282f9;
  background-color: transparent;
  color: white;
  font-weight: bold;
  font-size: 1.4rem;
  padding: 1rem;
  cursor: pointer;
}
</style>
