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
  </div>
</template>

<script>
export default {
  name: "Footer",
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
</style>