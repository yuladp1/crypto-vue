<template>
  <section class="page__change-fast change-fast">
    <div class="change-fast__wrapper _container">
      <div class="change-fast__content">
        <h1 class="_header-sections">Exchange funds in minutes</h1>
        <p>A wide range of digital asset trading and management services</p>
        <button class="button-blue">Launch App</button>
      </div>
      <img src="../assets/image-mobile.svg" alt="" />
    </div>
  </section>
</template>
<script>
export default {
  name: "changeMoneyFast",
};
</script>
<style scoped>
.change-fast {
  padding: 215px 0 76px 0;
  background: #f5f9fe;
  height: 520px;
}
.change-fast__wrapper {
  display: flex;
  align-items: center;
  gap: 49px;
  height: 100%;
  position: relative;
}
.change-fast__content {
  align-items: flex-start;
  flex: 0 1 40%;
}
.change-fast__content > *:not(:last-child) {
  margin-bottom: 32px;
}
p {
  font-size: 18px;
  font-weight: 500;
  line-height: 32px;
  color: #6f767e;
}
img {
  width: 500px;
  height: auto;
  position: absolute;
  bottom: 0;
  right: 50px;
}
@media (max-width: 980px) {
  .change-fast {
    padding: 80px 0 0 0;
    height: auto;
  }

  .change-fast__wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 50px;
  }
  .change-fast__content {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  img {
    width: 70%;
    height: auto;
    position: relative;
    right: auto;
  }
}
</style>
