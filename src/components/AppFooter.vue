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
        <div class="dc-logo"></div>
      </div>
    </div>
    <div class="footer__bottom">
      <button>SIGN-UP NOW!</button>
      <div class="social">
        <span class="follow-us">FOLLOW US</span>
        <span class="social-icon" v-for="(item , index) in contacts" :key="index">
         <img src="require(`../assets/${`item.name}` `)" alt="">
        </span>
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
      contacts: [
        {
          name: "footer-facebook.png",
        },
        {
          name: "footer-twitter.png",
        },
        {
          name: "footer-youtube.png",
        },
        {
          name: "footer-periscope.png",
        },
        {
          name: "footer-pinterest.png",
        },
      ]
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
      height: 90%;
      color: white;
      display: flex;
      flex-wrap: wrap;
      flex-direction: column;
      gap: 1rem;
      align-self: center;
    }

    .dc-logo {
      height: 300px;
      width: 400px;
      background-repeat: no-repeat;
      background-size: 400px;
      background-position: center;
      display: flex;
      background-image: url(../assets/dc-logo-bg.png);

      img {
        width: 400px;
        align-self: center;
      }
    }
  }

  &__bottom {
    height: 100px;
    background-color: #303030;
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;

    button {
      padding: 1rem 1.2rem;
      font-size: 1rem;
      font-weight: 600;
      color: white;
      background-color: #303030;
      border: 2px solid $blue;
    }

    .follow-us {
      color: $blue;
      font-size: 1.5rem;
      font-weight: 600;
      display: inline-block;
    }

    .social-icon {
        color: white;
        display: inline-block;
        width: 20px;
    }
  }
}
</style>
