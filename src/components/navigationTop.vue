<template>
  <div class="page__header header">
    <div class="header__wrapper">
      <figure class="header__logo">
        <img src="../assets/logo.svg" alt="logo" />
      </figure>
      <nav class="header__navigation" v-if="islargeScreen">
        <ul class="header__navigation-menu">
          <div>
            <li v-for="item in list1" :key="item.id">
              <a :href="item.scrollTo">{{ item.title }}</a>
            </li>
          </div>
        </ul>
      </nav>

      <div class="header__country">
        <figure class="header__country-flag">
          <img src="../assets/ukraine.svg" alt="" />
        </figure>
        <span class="header__country-name">Ukraine</span>
        <figure><img src="../assets/images/header-images/Vector.svg" alt="" /></figure>
      </div>

      <button class="header__button button-blue">Launch App</button>
      <figure class="header__menu-icon" v-if="!islargeScreen" v-on:click="toggleShowMenu">
        <img src="../assets/images/header-images/burger.svg" alt="" />
      </figure>
      <transition name="transition-content">
        <nav v-if="showMenu" :class="{ 'header__menu-drop': showMenu }">
          <ul>
            <li v-for="item in list1" :key="item.id">
              <a class="header__menu-drop-item" :href="item.scrollTo">{{ item.title }}</a>
            </li>
          </ul>
          <hr />
          <h2>Choose language</h2>
          <div class="header__menu-drop-countries">
            <div class="header__menu-drop-country">
              <figure class="header__menu-drop-country-flag">
                <img src="../assets/ukraine.svg" alt="" />
              </figure>
              <h2 class="header__menu-drop-country-name">Ukraine</h2>
            </div>
            <div class="header__menu-drop-country">
              <figure class="header__menu-drop-country-flag">
                <img src="../assets/ukraine.svg" alt="" />
              </figure>
              <span class="header__menu-drop-country-name">Ukraine</span>
            </div>
          </div>
        </nav>
      </transition>
    </div>
  </div>
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
      if (this.windowWidth >= 729) {
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
.header {
  position: relative;
}
.header__wrapper {
  padding: 0 24px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
}
.header__navigation {
  margin-left: 49px;
  margin-right: auto;
}
.header__navigation-menu > div {
  display: flex;
  gap: 40px;
}
.header__navigation-menu > li {
  display: inline-block;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #6f767e;
  padding: 30px 0;
}

.header__navigation-menu div > li > a {
  display: inline-block;
  padding: 30px 0;
  border-bottom: 2px solid white;
  color: #6f767e;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
}
.header__navigation-menu > div > li > a:hover {
  border-bottom: 2px solid #3e8bf3;
  color: #3e8bf3;
}
.header__country {
  display: flex;
  gap: 9px;
  align-items: center;
  margin-right: 24px;
}
.header__country > figure {
  display: flex;
  align-items: center;
  justify-content: center;
}
.header__country-name {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #000000;
}

.header__menu-icon {
  margin-left: 30px;
  z-index: 11;
}
.header__menu-drop {
  position: absolute;
  top: 0;
  right: 0;
  height: 1000px;
  width: 280px;
  padding: 84px 0 0 32px;
  background: white;
  display: flex;
  flex-direction: column;
  z-index: 10;
}
.header__menu-drop > ul {
  display: flex;
  gap: 24px;
  flex-direction: column;
}
.header__menu-drop > ul > li > a {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #6f767e;
}
.header__menu-drop > *:not(:last-child) {
  margin-bottom: 24px;
}
hr {
  height: 1px;
  width: auto;
  background: #d9d9d9;
  margin-right: 32px;
}

.header__menu-drop > h2 {
  font-weight: 500;
  font-size: 12px;
  line-height: 16px;
  color: #6f767e;
}

.header__menu-drop-countries {
  display: flex;
  flex-direction: column;
  gap: 20px;
  justify-content: flex-start;
}
.header__menu-drop-country {
  display: flex;
  gap: 8px;
  align-items: center;
  justify-content: flex-start;
}

.header__menu-drop-country-name {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  color: #6f767e;
}
.header__menu-drop-country-name:hover {
  color: black;
}

@media (max-width: 1000px) {
  .header__navigation-menu > div {
    gap: 20px;
    flex-wrap: wrap;
  }
}
@media (max-width: 900px) {
  .header__navigation-menu div > li > a {
    padding: 10px 0;
  }
}

@media (max-width: 729px) {
  .header__country {
    margin-left: auto;
  }
  .page__header {
    padding: 30px;
  }
}
@media (max-width: 500px) {
  .header__wrapper {
    gap: 30px;
  }
  .header__country {
    display: none;
  }
  .header__menu-icon {
    margin-left: 0;
  }
}
@media (max-width: 410px) {
  .header__wrapper {
    gap: 10px;
  }
  .header__menu-drop {
    width: 192px;
    height: 600px;
  }
  .header__menu-drop > a {
    font-size: 14px;
    line-height: 20px;
  }
  .header__menu-drop-country-name {
    font-size: 14px;
    line-height: 20px;
  }
}
</style>
