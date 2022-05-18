<template>
  <div class="content">
    <span> &ndash;&ndash;&gt; Content goes here &lt;&ndash;&ndash; </span>
  </div>
</template>

<script>
export default {
  name: "AppContent",
};
</script>

<style scoped lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";
.content {
  background-color: $black;
  height: 200px;
  display: flex;

  span {
    width: 100%;
    color: white;
    align-self: center;
    text-align: center;
    font-size: 2rem;
  }
}
</style>
