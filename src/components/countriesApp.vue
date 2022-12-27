<template>
  <div class="page__countries countries">
    <div class="coutries__wrapper _container" id="were-work">
      <figure class="map"><img src="../assets/map.svg" alt="" /></figure>
      <div class="countries__list">
        <div class="countries__list-country">
          <img src="../assets/images/countries-images/ukraine.svg" alt="" />
          <p class="country-name">Ukraine</p>
        </div>
        <div class="countries__list-country">
          <img src="../assets/images/countries-images/kazakhstan.svg" alt="" />
          <p class="country-name">Kazakhstan</p>
        </div>
        <div class="countries__list-country">
          <img src="../assets/images/countries-images/turkey.svg" alt="" />
          <p class="country-name">Turkey</p>
        </div>
        <div class="countries__list-country">
          <img src="../assets/images/countries-images/ukraine.svg" alt="" />
          <p class="country-name">Ukraine</p>
        </div>
      </div>

      <section class="countries__content">
        <h2 class="_header-sections">
          Countries with which the service is already working
        </h2>
        <div class="countries__content-buttons">
          <button class="button-blue">Launch App</button>
          <button class="button-country button-blue">Connect my country</button>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.countries {
  padding: 120px 0;
}
.coutries__wrapper {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  position: relative;
  /* height: 568px; */
}
.map {
  position: absolute;
  top: 0;
  right: 0;
  width: 100%;
}
.map > img {
  width: 100%;
  height: 100%;
  top: 0;
  right: 0;
  object-fit: cover;
}
.countries__content {
  display: flex;
  flex-direction: column;
  z-index: 1;
}
.countries__content > h2 {
  display: inline-block;
  max-width: 452px;
}
.countries__content-buttons {
  display: flex;
  gap: 16px;
  padding-top: 32px;
}
.button-country {
  border: 1px solid #f5f9fe;
  background: #f5f9fe;
  color: #6f767e;
}
.button-country:hover {
  border: 1px solid #e3eefd;
  background: #e3eefd;
  color: black;
}
.button-country:active {
  border: 1px solid #bfd8fb;
  background: #bfd8fb;
  color: black;
}
.countries__list {
  display: flex;
  flex-direction: column;
  gap: 5px;
  padding: 8px;
  background: #f5f9fe;
  max-width: 157px;
  border-radius: 16px;
  z-index: 1;
}
.countries__list-country {
  display: flex;
  gap: 8px;
  justify-items: center;
  align-items: center;
  border-radius: 8px;
  padding: 10px 16px;
  color: #6f767e;
}
.countries__list-country:hover {
  background-color: white;
  cursor: pointer;
  color: black;
}
.country-name {
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 150%;
  color: inherit;
}
@media (max-width: 800px) {
  .countries {
    padding: 80px 0;
  }
  .coutries__wrapper {
    flex-direction: column;
    justify-content: space-between;
  }
  .map {
    position: relative;
    order: 2;
  }
  .countries__content {
    order: 1;
  }
  .countries__content > h2 {
    max-width: 503px;
  }
  .countries__list {
    order: 3;
    flex-direction: row;
  }
}
@media (max-width: 400px) {
  .countries__content-buttons {
    flex-direction: column;
    gap: 8px;
    padding-top: 20px;
  }
}
</style>
