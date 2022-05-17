<template>
  <div class="footer">
    <div class="container">
      <div class="footer__top">
        <div class="footer-link">
          <h3>DC COMICS</h3>
          <ul>
            <li v-for="(item, index) in dcComics" :key="index">
              <a href="">{{ item.name }}</a>
            </li>
          </ul>
          <h3>SHOP</h3>
          <ul>
            <li v-for="(item, index) in shop" :key="index">
              <a href="">{{ item.name }}</a>
            </li>
          </ul>
          <h3>DC</h3>
          <ul>
            <li v-for="(item, index) in DC" :key="index">
              <a href="">{{ item.name }}</a>
            </li>
          </ul>
          <h3>SITES</h3>
          <ul>
            <li v-for="(item, index) in sites" :key="index">
              <a href="">{{ item.name }}</a>
            </li>
          </ul>
        </div>
        <div class="dc-logo">
          <img src="../assets/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppFooter",
  data: function () {
    return {
      dcComics: [
        {
          name: "Characters",
        },
        {
          name: "Comics",
        },
        {
          name: "Movies",
        },
        {
          name: "TV",
        },
        {
          name: "Games",
        },
        {
          name: "Videos",
        },
        {
          name: "News",
        },
      ],
      shop: [
        {
          name: "Shop DC",
        },
        {
          name: "Shop DC Collectibles",
        },
      ],
      DC: [
        {
          name: "Terms of Use",
        },
        {
          name: "Privacy policy(New)",
        },
        {
          name: "Ad Choices",
        },
        {
          name: "Advertising",
        },
        {
          name: "Jobs",
        },
        {
          name: "Subscriptions",
        },
        {
          name: "Talent Workshops",
        },
        {
          name: "CPSC Certificates",
        },
        {
          name: "Ratings",
        },
        {
          name: "Shop Help",
        },
        {
          name: "Contact Us",
        },
      ],
      sites: [
        {
          name: "DC",
        },
        {
          name: "MAD Magazine",
        },
        {
          name: "DC Kids",
        },
        {
          name: "DC Universe",
        },
        {
          name: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";

.footer {
  background-image: url(../assets/footer-bg.jpg);

  &__top {
    height: 300px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    .footer-link {
      height: 85%;
      color: white;
      display: flex;
      flex-wrap: wrap;
      flex-direction: column;
      gap: 1rem;
      align-self: center;
    }

    .dc-logo {
      height: 300px;
      display: flex;

      img {
        width: 400px;
        align-self: center;
      }
    }
  }
}
</style>
