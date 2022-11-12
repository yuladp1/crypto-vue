<template>
  <nav>
    <figure class="logo-image"></figure>
    <div class="container-button-and-menu">
      <button>Launch App</button>
      <figure class="menu-image"></figure>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navigationTop",
  data() {},
  methods: {},
};
</script>
<style scoped>
figure {
  display: block;
  margin-block-start: 0;
  margin-block-end: 0;
  margin-inline-start: 0;
  margin-inline-end: 0;
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 68px;
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
</style>
