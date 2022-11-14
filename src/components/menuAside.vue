<template>
  <aside>
    <nav>
      <ul>
        <div v-for="l in list" :key="l.id">
          <li>{{ l }}</li>
        </div>
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
  </aside>
</template>

<script>
export default {
  data() {
    return {
      list: ["About", "How does it works", "Were we work", "FAQ", "Contacts"],
    };
  },
};
</script>

<style scoped>
aside {
  width: 192px;
  height: 600px;
}
nav {
  width: 100%;
  height: 100%;
}
ul {
  margin-block-start: 0;
  margin-block-end: 0;
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  padding-inline-start: 0px;
  margin: 70px auto 24px 24px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
  width: 144px;
  height: 200px;
  padding-bottom: 24px;
  border-bottom: 1px solid #d9d9d9;
}
li {
  list-style-type: none;
  color: black;
  width: 100%;
  height: 20px;
  margin-bottom: 24px;
  font-size: 14px;
  font-weight: 500px;
  line-height: 20px;
  color: #6f767e;
}
h2 {
  font-size: 12px;
  font-weight: 500px;
  line-height: 16px;
  color: #6f767e;
  margin: 24px auto 24px 24px;
}
.countries-list {
  display: flex;
  flex-direction: column;
}
.wrapper-country {
  display: flex;
  justify-items: center;
  align-items: center;
  height: 36px;
  border-radius: 8px;
  margin: 8px 16px 8px 16px;
}
.img-flag {
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
.country-name {
  font-size: 14px;
  font-weight: 500;
  color: #6f767e;
}
</style>
