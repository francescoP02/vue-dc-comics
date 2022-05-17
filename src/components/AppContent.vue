<template>
  <div class="content">
    <span> --> Content goes here </span>
  </div>
</template>

<script>
export default {
  name: "AppContent",
};
</script>

<style scoped lang="scss">
.content {
  background-color: black;
  height: 150px;
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
