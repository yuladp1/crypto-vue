<template>
  <section class="page__transfer transfer">
    <div class="transfer__wrapper _container">
      <div class="transfer__content">
        <h1 class="transfer__content-title">Exchange crypto and fiat without limits</h1>
        <button class="transfer__content-button button-blue">Launch App</button>
        <p class="transfer__content-text">Works on smart contracts</p>
      </div>

      <div class="transfer__wrapper-form">
        <div class="transfer__form">
          <div class="transfer__form__buttons buttons-form">
            <button class="buttons-form__black">Send</button>
            <button class="buttons-form__white">Recieve</button>
          </div>
          <div class="transfer__form-currency currency">
            <div class="currency__wrapper">
              <p class="currency__amount">$350.00</p>
              <p class="currency__exchange-rate">0 BTC ≈ $0.00</p>
            </div>
            <div class="currency__button">
              <img src="../assets/images/transfer-images/arrows.svg" alt="" />
            </div>
          </div>

          <form class="transfer__inputs">
            <div class="transfer__inputs-wrapper-input">
              <label>Pay with</label>
              <select>
                <option class="bitcoin">Bitcoin</option>
                <option>Currency2</option>
                <option>Currency3</option>
              </select>
            </div>
            <div class="transfer__inputs-wrapper-input">
              <label>Send to</label>
              <input class="input-phone" type="text" placeholder="+995 590 558 124" />
            </div>
            <div class="transfer__inputs-wrapper-input">
              <label>Note</label>
              <input type="text" placeholder="Type to add a note" />
            </div>
          </form>
          <div class="button-continue-transfer button-blue">Continue transfer</div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "transferContinue",
};
</script>
<style scoped>
.transfer {
  background: #f5f9fe;
}
.transfer__wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.transfer__content {
  flex: 0 1 50%;
  justify-items: flex-start;
  padding: 75px 0 47px 0;
}
.transfer__content > *:not(:last-child) {
  margin-bottom: 32px;
}
.transfer__content-title {
  font-weight: 500;
  font-size: 64px;
  line-height: 72px;
  color: #000000;
}
.transfer__content-button {
  font-size: 20px;
  line-height: 32px;
}
.transfer__content-text {
  font-weight: 500;
  font-size: 16px;
  line-height: 150%;
  color: #6f767e;
  padding-left: 32px;
  position: relative;
}
.transfer__content-text::before {
  content: "";
  width: 24px;
  height: 24px;
  background-image: url("../assets/images/transfer-images/ClipboardText.svg");
  background-position: center;
  position: absolute;
  left: 0;
}
.transfer__wrapper-form {
  flex: 0 1 auto;
  background-image: url("../assets/images/transfer-images/blueCircle.png");
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 75px;
  margin: 75px 0 47px 0;
}
.transfer__form {
  background: white;
  padding: 19.19px 18.39px 18.14px 19.61px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 455px;
  position: relative;
}
.transfer__form::before {
  content: "";
  width: 143px;
  height: 135px;
  background-image: url("../assets/images/transfer-images/usdCoin.png");
  background-position: center;
  background-size: cover;
  position: absolute;
  left: -72px;
  top: -66px;
  z-index: 1;
}
.transfer__form::after {
  content: "";
  width: 120px;
  height: 129px;
  background-image: url("../assets/images/transfer-images/ethereumCoin.png");
  background-position: center;
  position: absolute;
  right: -60px;
  bottom: -60px;
  z-index: 1;
}

.buttons-form {
  display: flex;
  gap: 20px;
}
.buttons-form__black,
.buttons-form__white {
  font-family: "Inter";
  font-style: normal;
  font-weight: 700;
  font-size: 9.30594px;
  line-height: 150%;
  padding: 7px 21px;
  border-radius: 6.20396px;
}
.buttons-form__black {
  background: #000000;
  color: #ffffff;
}
.buttons-form__white {
  background: white;
  color: black;
}
.transfer__form-currency {
  display: flex;
  justify-content: center;
  margin: 46.5px 0;
  position: relative;
  width: 100%;
}
.currency__wrapper {
  display: flex;
  justify-content: center;
  flex-direction: column;
}
.currency__amount {
  font-weight: 800;
  font-size: 43.4277px;
  line-height: 53px;
  color: #000000;
}
.currency__exchange-rate {
  font-weight: 400;
  font-size: 10.8569px;
  line-height: 150%;
  text-align: center;
  color: #5d5d5b;
}
.currency__button {
  position: absolute;
  right: 0;
  top: 14.5px;
}
.transfer__inputs {
  display: flex;
  flex-direction: column;
  background: #f5f9fe;
  border-radius: 12.4079px;
  width: 100%;
  padding: 0 24px;
  position: relative;
}
.transfer__inputs > *:not(:last-child) {
  border-bottom: 1.16126px solid rgba(207, 219, 213, 0.6);
}

.transfer__inputs-wrapper-input {
  padding: 21px 0;
  min-height: 41px;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.transfer__inputs-wrapper-input > label {
  font-weight: 500;
  font-size: 9.30594px;
  line-height: 150%;
  color: #5d5d5b;
  flex: 0 1 30%;
}
.transfer__inputs-wrapper-input > input,
.transfer__inputs-wrapper-input > select {
  background: #f5f9fe;
  flex: 0 1 70%;
}
.input-phone {
  font-weight: 700;
  font-size: 10.8569px;
  line-height: 16px;
  color: black;
}

select {
  appearance: none;
  border: none;
  padding: 0;
  width: 100%;
  font-weight: 700;
  font-size: 10.8569px;
  line-height: 16px;
  position: relative;
}
select::after {
  position: absolute;
  right: 0;
  top: 0;
  content: "";
  width: 0.8em;
  height: 0.5em;
  background-color: var(--select-arrow);
  clip-path: polygon(100% 0%, 0 0%, 50% 100%);
}
.bitcoin {
  position: relative;
  padding-left: 20px;
}
.bitcoin::before {
  width: 14px;
  height: 14px;
  background-image: url("../assets/images/transfer-images/BitcoinSmall.svg");
  background-position: center;
  position: absolute;
  left: 0;
}
.button-continue-transfer {
  font-weight: 700;
  font-size: 10.8569px;
  line-height: 16px;
  padding: 12px 62.5px;
  margin: 21px auto;
}
</style>
