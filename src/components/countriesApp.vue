<template>
  <section>
    <h1>Страны, с которыми уже работает сервис</h1>
    <button class="button-launch-app">Launch App</button>
    <button class="button-country">Подключить мою страну</button>
    <figure class="image-map"><img src="../assets/map.svg" alt="" /></figure>
  </section>
  <div class="countries-list">
    <div class="wrapper-country">
      <figure class="img-flag"></figure>
      <p class="country-name">Ukraine</p>
    </div>
    <div class="wrapper-country">
      <figure class="img-flag"></figure>
      <p class="country-name">Ukraine</p>
    </div>
    <div class="wrapper-country">
      <figure class="img-flag"></figure>
      <p class="country-name">Ukraine</p>
    </div>
    <div class="wrapper-country">
      <figure class="img-flag"></figure>
      <p class="country-name">Ukraine</p>
    </div>
    <div class="wrapper-country">
      <figure class="img-flag"></figure>
      <p class="country-name">Ukraine</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  section {
    margin: 32px 16px 54px 16px;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  h1 {
    font-size: 24px;
    font-weight: 700;
    line-height: 32px;
  }
  button {
    width: 100%;
    height: 48px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 16px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 32px 0 32px 0;
  }
  .image-map {
    width: 100%;
    height: 166px;
    margin: 32px 0 32px 0;
    margin-block-start: 0;
    margin-block-end: 0;
    margin-inline-start: 0;
    margin-inline-end: 0;
  }
  img {
    width: 100%;
    height: 100%;
  }
  .countries-list {
    width: 100%;
    height: 52px;
    display: flex;
    align-items: center;
    overflow: hidden;
    margin-bottom: 36px;
    background-color: #f5f9fe;
  }
  .wrapper-country {
    display: flex;
    justify-items: center;
    align-items: center;
    height: 36px;
    border-radius: 8px;
    margin: 8px 16px 8px 16px;
  }
  .wrapper-country:hover {
    background-color: white;
    cursor: pointer;
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
    padding-right: 16px;
  }
}
</style>
