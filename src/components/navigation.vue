<template>
  <nav>
    <figure class="logo-image"></figure>
    <MenuAside v-if="islargeScreen" v-bind:list="list" />
    <div class="container-button-and-menu">
      <button>Launch App</button>
      <figure class="menu-image" v-on:click="toggleShowMenu"></figure>
    </div>
    <MenuAside v-if="showMenu" v-bind:list="list" />
  </nav>
</template>

<script>
import MenuAside from "./MenuAside.vue";
export default {
  name: "navigationTop",
  components: { MenuAside },

  data() {
    return {
      showMenu: false,
      list: ["About", "How does it works", "Were we work", "FAQ", "Contacts"],
    };
  },
  methods: {
    toggleShowMenu() {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>
<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  figure {
    display: block;
    margin-block-start: 0;
    margin-block-end: 0;
    margin-inline-start: 0;
    margin-inline-end: 0;
    z-index: 7;
  }
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 68px;
    position: relative;
  }
  nav .logo-image {
    width: 97px;
    height: 24px;
    margin-left: 16px;
    background-size: contain;
    background-image: url("../assets/logo.svg");
  }
  nav .menu-image {
    width: 24px;
    height: 24px;
    margin-left: 16px;
    margin-right: 16px;
    background-image: url("../assets/List.svg");
  }
  nav button {
    width: 100px;
    height: 34px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 14px;
    font-weight: 500;
    color: white;
    margin-right: 0;
  }
  .container-button-and-menu {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    width: 50%;
  }
}
@media screen and (min-width: 721px) and (max-width: 1440px) {
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 68px;
    position: relative;
    background-color: white;
  }
  figure {
    display: block;
    margin-block-start: 0;
    margin-block-end: 0;
    margin-inline-start: 0;
    margin-inline-end: 0;
    z-index: 7;
  }
  nav .logo-image {
    width: 129px;
    height: 32px;
    margin-left: 24px;
    background-size: contain;
    background-image: url("../assets/logo.svg");
  }
  .container-button-and-menu {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    width: 50%;
  }
  nav button {
    width: 121px;
    height: 48px;
    font-size: 16px;

    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-weight: 500;
    color: white;
    margin-right: 0;
  }
  nav .menu-image {
    width: 32px;
    height: 32px;
    margin-left: 24px;
    margin-right: 24px;
    background-image: url("../assets/List.svg");
  }
}

@media screen and (min-width: 1441px) {
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 88px;
    background-color: white;
  }

  nav .logo-image {
    width: 129px;
    height: 32px;
    margin-left: 24px;
    background-size: contain;
    background-image: url("../assets/logo.svg");
  }
  nav button {
    width: 121px;
    height: 48px;
    font-size: 16px;

    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-weight: 500;
    color: white;
    margin-right: 0;
  }
  nav .menu-image {
    display: none;
  }
}
</style>
