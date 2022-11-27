<template>
  <nav>
    <figure class="logo-image"></figure>
    <nav v-if="islargeScreen" class="menu-large-screen">
      <ul class="menu-large-screen-ul">
        <li v-for="item in list1" :key="item.id">
          <p>
            <a :href="item.scrollTo">{{ item.title }}</a>
          </p>
        </li>
      </ul>
    </nav>

    <div class="container-button-and-menu">
      <div class="large-screen-countries-list" v-if="islargeScreen">
        <div class="large-screen-wrapper-country">
          <figure class="large-screen-img-flag"></figure>
          <p class="large-screen-country-name">Ukraine</p>
        </div>
        <div class="large-screen-wrapper-country">
          <figure class="large-screen-img-flag"></figure>
          <p class="large-screen-country-name">Ukraine</p>
        </div>
      </div>
      <button>Launch App</button>
      <figure
        class="menu-image"
        v-if="!islargeScreen"
        v-on:click="toggleShowMenu"
      ></figure>
    </div>

    <nav v-if="showMenu" class="menu-medium-screen">
      <ul>
        <li v-for="item in list1" :key="item.id">
          <p>
            <a :href="item.scrollTo">{{ item.title }}</a>
          </p>
        </li>
      </ul>
      <h2>Choose language</h2>
      <div class="countries-list">
        <div class="wrapper-country">
          <figure class="img-flag"></figure>
          <p class="country-name">Ukraine</p>
        </div>
        <div class="wrapper-country">
          <figure class="img-flag"></figure>
          <p class="country-name">Ukraine</p>
        </div>
      </div>
    </nav>
  </nav>
</template>

<script>
export default {
  name: "navigationTop",
  components: {},

  data() {
    return {
      showMenu: false,
      islargeScreen: false,
      list1: [
        { title: "About", scrollTo: "#about" },
        { title: "How does it works", scrollTo: "#how-work" },
        { title: "Were we work", scrollTo: "#were-work" },
        { title: "FAQ", scrollTo: "#faq" },
        { title: "Contacts", scrollTo: "#contacts" },
      ],
      windowWidth: null,
    };
  },
  created() {
    this.checkScreen();
    window.addEventListener("resize", this.checkScreen);
  },
  methods: {
    toggleShowMenu() {
      this.showMenu = !this.showMenu;
    },
    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth >= 1441) {
        this.islargeScreen = true;
        this.showMenu = false;
        return;
      } else {
        this.islargeScreen = false;
        return;
      }
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
  .menu-medium-screen {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 0;
    right: 0;
    background-color: white;
    width: 192px;
    height: 600px;
    z-index: 6;
  }
  .menu-medium-screen > ul {
    margin: 70px auto 24px 24px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    width: 144px;
    height: auto;
    padding-bottom: 24px;
    border-bottom: 1px solid #d9d9d9;
    list-style-type: none;
  }
  .menu-medium-screen > ul li {
    text-decoration: none;
  }

  .menu-medium-screen > p {
    list-style-type: none;
    color: black;
    width: 100%;
    margin-bottom: 24px;
    font-size: 14px;
    font-weight: 500px;
    line-height: 20px;
    color: #6f767e;
  }
  .menu-medium-screen > h2 {
    font-size: 12px;
    font-weight: 500px;
    line-height: 16px;
    color: #6f767e;
    margin: 24px auto 24px 24px;
  }
  .menu-medium-screen .countries-list {
    display: flex;
    flex-direction: column;
  }
  .menu-medium-screen .wrapper-country {
    display: flex;
    justify-items: center;
    align-items: center;
    height: 36px;
    border-radius: 8px;
    margin: 8px 16px 8px 16px;
  }
  .menu-medium-screen .img-flag {
    background-image: url("../assets/ukraine.svg");
    background-repeat: no-repeat;
    background-position: center;
    padding-right: 8px;
    padding-left: 8px;
    width: 20px;
    height: 20px;
    margin-block-start: 0;
    margin-block-end: 0;
    margin-inline-start: 0;
    margin-inline-end: 0;
  }
  .menu-medium-screen .country-name {
    font-size: 14px;
    font-weight: 500;
    color: #6f767e;
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
  .menu-medium-screen {
    display: flex;
    flex-direction: column;
    justify-items: flex-start;
    justify-content: flex-start;
    width: 280px;
    height: 1000px;
    z-index: 6;
    position: absolute;
    top: 0;
    right: 0;
    background-color: white;
    z-index: 6;
  }
  .menu-medium-screen > ul {
    margin-block-start: 0;
    margin-block-end: 0;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    padding-inline-start: 0px;
    margin: 84px auto 24px 32px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-start;
    width: auto;
    height: auto;
    padding-bottom: 24px;
    border-bottom: 1px solid #d9d9d9;
    list-style-type: none;
    background-color: white;
  }
  .menu-medium-screen > ul li {
    text-decoration: none;
  }

  .menu-medium-screen > p {
    list-style-type: none;
    color: black;
    width: 100%;
    margin-bottom: 24px;
    font-size: 16px;
    font-weight: 500px;
    line-height: 24px;
    color: #6f767e;
  }
  .menu-medium-screen > h2 {
    font-size: 12px;
    font-weight: 500px;
    line-height: 16px;
    color: #6f767e;
    margin: 24px auto 24px 24px;
  }
  .menu-medium-screen .countries-list {
    display: flex;
    flex-direction: column;
  }
  .menu-medium-screen .wrapper-country {
    display: flex;
    justify-items: center;
    align-items: center;
    height: 36px;
    border-radius: 8px;
    margin: 8px 16px 8px 16px;
  }
  .menu-medium-screen .img-flag {
    background-image: url("../assets/ukraine.svg");
    background-repeat: no-repeat;
    background-position: center;
    padding-right: 8px;
    padding-left: 8px;
    width: 20px;
    height: 20px;
    margin-block-start: 0;
    margin-block-end: 0;
    margin-inline-start: 0;
    margin-inline-end: 0;
  }
  .menu-medium-screen .country-name {
    font-size: 16px;
    line-height: 34px;
    font-weight: 500;
    color: #6f767e;
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
}
.menu-large-screen {
  display: flex;
  justify-content: space-between;
}
.menu-large-screen-ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-grow: 1;
  gap: 40px;
  border-bottom: 1px solid #d9d9d9;
  list-style-type: none;
  background-color: white;
}
.menu-large-screen > li {
  text-decoration: none;
  font-size: 16px;
}
.container-button-and-menu {
  display: flex;

  gap: 15px;
}
.large-screen-countries-list {
  display: flex;
  gap: 10px;
}
.large-screen-wrapper-country {
  display: flex;
  gap: 10px;
  align-items: center;
  gap: 10px;
}
.large-screen-img-flag {
  width: 20px;
  height: 20px;
  background-image: url("../assets/ukraine.svg");
  background-repeat: no-repeat;
  background-position: center;
}
</style>
