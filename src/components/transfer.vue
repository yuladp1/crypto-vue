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
          <form>
            <div class="wrapper-form-all">
              <div class="wrapper-label-input">
                <label>Pay with</label>
                <select>
                  <option>Bitcoin</option>
                  <option>Currency2</option>
                  <option>Currency3</option>
                </select>
              </div>
              <div class="wrapper-label-input">
                <label>Send to</label>
                <input type="text" />
              </div>
              <div class="wrapper-label-input wrapper-label-input-last">
                <label>Note</label>
                <input type="text" placeholder="Type to add a note" />
              </div>
            </div>
            <button class="button-continue-transfer">Continue transfer</button>
          </form>
        </div>
      </div>
      <img src="../assets/blue_arrow.svg" alt="" class="blue-arrow" />
      <img src="../assets/bluecoin.svg" alt="" class="blue-coin" />
    </div>
    <div class="empty-block"></div>
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
@media screen and (min-width: 320px) and (max-width: 720px) {
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
    bottom: -65px;
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
    bottom: -90px;
    left: 55%;
    width: 67px;
    height: 76px;
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
    margin: 15px auto;
    background-color: #ffffff;
    position: absolute;
    top: 27px;
    z-index: 2;
    border-radius: 7.02px;
    box-shadow: 0px 6.001938819885254px 12.003877639770508px 0px #00000014;
  }
  .wrapper-buttons,
  .wrapper-amount-change {
    display: flex;
    justify-items: center;
    width: 140px;
    margin: auto;
    position: relative;
  }
  .wrapper-buttons {
    margin-top: 19.73px;
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
  .empty-block {
    width: 100%;
    height: 100px;
    background-color: #f5f9fe;
  }
  form {
    display: flex;
    flex-direction: column;
    margin: 0 16px;
    width: auto;
  }
  .wrapper-form-all {
    background-color: #f5f9fe;
    border-radius: 9.36px;
  }
  label {
    width: 70px;
    font-size: 9.31px;
    font-weight: 500;
    line-height: 14px;
    color: #5d5d5b;
  }

  input,
  select {
    width: 140px;
    height: 43px;
    font-size: 11px;
    font-weight: 700;
    line-height: 16.22px;
    background-color: #f5f9fe;
    border: none;
  }
  input::placeholder {
    font-size: 11px;
    font-weight: 400;
    line-height: 16.22px;
  }
  .wrapper-label-input {
    display: flex;
    height: 48px;
    align-items: center;
    margin: 0 18px 0 16px;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  .wrapper-label-input-last {
    border-bottom: none;
  }
  .button-continue-transfer {
    width: 100%;
    height: 41px;
    border-radius: 6.2px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 14px;
    font-weight: 700;
    color: white;
    display: block;
    margin: 11px 0 16px 0;
  }
}
@media screen and (min-width: 721px) and (max-width: 1440px) {
  section {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
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
    left: 48%;
    rotate: 3deg;
    width: 235px;
    height: 215px;
  }
  .blue-arrow {
    position: absolute;
    bottom: -63px;
    right: 45%;
    rotate: 344deg;
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
    bottom: -90px;
    left: 55%;
    width: 67px;
    height: 76px;
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
    margin: 15px auto;
    background-color: #ffffff;
    position: absolute;
    top: 27px;
    z-index: 2;
    border-radius: 7.02px;
    box-shadow: 0px 6.001938819885254px 12.003877639770508px 0px #00000014;
  }
  .wrapper-buttons,
  .wrapper-amount-change {
    display: flex;
    justify-items: center;
    width: 140px;
    margin: auto;
    position: relative;
  }
  .wrapper-buttons {
    margin-top: 19.73px;
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
  .empty-block {
    display: none;
  }
  form {
    display: flex;
    flex-direction: column;
    margin: 0 16px;
    width: auto;
  }
  .wrapper-form-all {
    background-color: #f5f9fe;
    border-radius: 9.36px;
  }
  label {
    width: 70px;
    font-size: 9.31px;
    font-weight: 500;
    line-height: 14px;
    color: #5d5d5b;
  }

  input,
  select {
    width: 140px;
    height: 43px;
    font-size: 11px;
    font-weight: 700;
    line-height: 16.22px;
    background-color: #f5f9fe;
    border: none;
  }
  input::placeholder {
    font-size: 11px;
    font-weight: 400;
    line-height: 16.22px;
  }
  .wrapper-label-input {
    display: flex;
    height: 48px;
    align-items: center;
    margin: 0 18px 0 16px;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  .wrapper-label-input-last {
    border-bottom: none;
  }
  .button-continue-transfer {
    width: 100%;
    height: 41px;
    border-radius: 6.2px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 14px;
    font-weight: 700;
    color: white;
    display: block;
    margin: 11px 0 16px 0;
  }
}
</style>
