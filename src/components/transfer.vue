<template>
  <section>
    <div class="wrapper-continue-transfer">
      <img src="../assets/green_arrow.svg" alt="" class="green-arrow" />
      <img src="../assets/usd.svg" alt="" class="green-coin" />
      <img src="../assets/bsd.svg" alt="" class="yellow-coin" />
      <figure>
        <img src="../assets/blueCircle.svg" alt="" />
      </figure>
      <div class="continue-transfer">
        <div class="wrapper-buttons">
          <button class="send">Send</button>
          <button class="recieve">Recieve</button>
        </div>
        <div class="wrapper-amount-change">
          <p class="amount">$350.00</p>
          <p class="exchange-rate">0 BTC ≈ $0.00</p>
          <button class="change-currency" />
        </div>
      </div>
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
.wrapper-buttons,
.wrapper-amount-change {
  display: flex;
  justify-items: center;
  width: 140px;
  margin: auto;
  position: relative;
}
.wrapper-amount-change {
  flex-direction: column;
  align-items: center;
  width: 100%;
}
.send,
.recieve {
  font-size: 12px;
  font-weight: 400;
  padding: 7px;
  color: black;
  background-color: #ffffff;
  border-radius: 6.2px;
  border: 1px solid white;
  width: 65px;
}
.send:hover,
.recieve:hover {
  color: white;
  background-color: black;
  border-radius: 6.2px;
  border: 1px solid black;
}
.recieve {
  margin-left: 10px;
}
.change-currency {
  background-color: white;
  background-image: url("../assets/icon.svg");
  background-size: 14px 11px;
  background-position: center;
  background-repeat: no-repeat;
  width: 30.4px;
  height: 30.4px;
  border: 1px solid #cfdbd5;
  border-radius: 4.68px;
  position: absolute;
  top: 40px;
  right: 16px;
  margin: 0;
}
.amount {
  font-size: 33px;
  font-weight: 800;
  line-height: 40px;
  margin: 27px 0 0 0;
}
.exchange-rate {
  margin-block-start: 0;
  font-size: 8.2px;
  font-weight: 400;
  line-height: 12.28px;
  color: #5d5d5b;
}
</style>
