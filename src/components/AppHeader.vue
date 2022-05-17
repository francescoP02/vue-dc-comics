<template>
  <div class="container header">
    <div class="header__logo">
      <img src="../assets/dc-logo.png" alt="" />
    </div>
    <nav>
      <ul class="header__menu">
        <li
          v-for="(item, index) in menuItem"
          :key="index"
          :class="{ active: item.active }"
        >
          <a href="">{{ item.name }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      menuItem: [
        {
          name: "CHARACTERS",
          active: false,
        },
        {
          name: "COMICS",
          active: true,
        },
        {
          name: "MOVIES",
          active: false,
        },
        {
          name: "TV",
          active: false,
        },
        {
          name: "GAMES",
          active: false,
        },
        {
          name: "COLLECTIBLES",
          active: false,
        },
        {
          name: "VIDEOS",
          active: false,
        },
        {
          name: "FANS",
          active: false,
        },
        {
          name: "NEWS",
          active: false,
        },
        {
          name: "SHOP",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../style/common.scss";
@import "../style/variables.scss";

.header {
  display: flex;
  flex-direction: row;
  height: 100px;
  justify-content: space-between;

  &__logo {
    img {
      width: 80px;
    }
  }

  &__menu {
    display: flex;
    align-self: center;

    li {
      margin: 0.5rem;
      padding: 0.5rem;
      color: $nav-element;
      line-height: 50px;

      &.active {
        color: $active-nav-element;
        border-bottom: 5px solid $active-nav-element;
      }
    }
  }
}
</style>
