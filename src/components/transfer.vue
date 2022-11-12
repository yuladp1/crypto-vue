<template>
  <section>
    <div class="wrapper-continue-transfer">
      <img src="../assets/green_arrow.svg" alt="" class="green-arrow" />
      <img src="../assets/usd.svg" alt="" class="green-coin" />
      <img src="../assets/bsd.svg" alt="" class="yellow-coin" />
      <figure>
        <img src="../assets/blueCircle.svg" alt="" />
      </figure>
      <div class="continue-transfer"></div>
      <img src="../assets/blue_arrow.svg" alt="" class="blue-arrow" />
      <img src="../assets/bluecoin.svg" alt="" class="blue-coin" />
    </div>
  </section>
</template>

<script>
export default {
  name: "transferContinue",
  data() {},
  methods: {},
};
</script>
<style scoped>
.wrapper-continue-transfer {
  width: 100%;
  height: 418px;
  background-color: #f5f9fe;
  position: relative;
  display: flex;
  justify-content: center;
}
.green-arrow {
  position: absolute;
  top: -40px;
  left: 45%;
  rotate: 3deg;
  width: 235px;
  height: 215px;
}
.blue-arrow {
  position: absolute;
  bottom: -40px;
  right: 45%;
  rotate: 3deg;
  width: 235px;
  height: 215px;
}
.green-coin {
  position: absolute;
  top: -35px;
  right: 60%;
  width: 92px;
  height: 82px;
  z-index: 3;
}
.yellow-coin {
  position: absolute;
  top: -45px;
  right: 50%;
  width: 34px;
  height: 35px;
}
.blue-coin {
  position: absolute;
  bottom: -75px;
  left: 55%;
  width: 90px;
  height: 95px;
}
figure {
  position: absolute;
  top: 0;
  width: 100%;
  height: 418px;
}
img {
  height: 100%;
  width: auto;
  width: 100%;
}
.continue-transfer {
  height: 362px;
  min-width: 288px;
  margin: 0 auto;
  background-color: #ffffff;
  position: absolute;
  top: 27px;
  z-index: 2;
}
</style>
