<template>
    <div class="content">
      <div class="product">
        <img :src="productObj.thumb" alt="" />
        <h4>{{ productObj.series }}</h4>
      </div>
  </div>
</template>

<script>
export default {
  name: "AppContent",
  // Passare i valori come un'oggetto unico in due modi: object notation oppure array di stringhe
  props: {
    productObj: Object,
  },
};
</script>

<style scoped lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";

.content {
  width: calc(100% / 6);

  .product {
    padding: 1rem 0.5rem;
    position: relative;
    width: 100%;

    h4 {
      font-size: 1rem;
      position: absolute;
      color: white;
      text-transform: uppercase;
      position: absolute;
      top: 65%;
      background-color: #1c1c1c;
      width: calc(100% - 1rem);
      height: calc(35% - 1rem);
    }
  }
  
}
</style>
