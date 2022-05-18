<template>
  <div class="shop">
    <div class="container">
      <div class="shop-item" v-for="(item,index) in shopItem" :key="index">
        <img :src="require(`../assets/img/${item.img}`)" alt="">
        <span> {{item.name}} </span>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "AppShop",
  data: function() {
    return {
      shopItem: [
        {
          img: "buy-comics-digital-comics.png",
          name: "digital comics",
        },
        {
          img: "buy-comics-merchandise.png",
          name: "dc merchandise",
        },
        {
          img: "buy-comics-subscriptions.png",
          name: "subscription",
        },
        {
          img: "buy-comics-shop-locator.png",
          name: "comic shop locator",
        },
        {
          img: "buy-dc-power-visa.svg",
          name: "dc power visa",
        },
      ],
    }
  }
};
</script>

<style scoped lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";

.shop {
  background-color: $blue;
  display: flex;

  .container {

    display: flex;
    .shop-item {
      padding: 3rem 1rem;
      width: calc(100% / 5);
      display: flex;
      flex-direction: row;
      align-items: center;

      img {
        width: 20%;
      }

      span {
        padding-left: 1rem;
        color: white;
        text-transform: uppercase;
        text-align: center;
      }
    }
  }

}
</style>
