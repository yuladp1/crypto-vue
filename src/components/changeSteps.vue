<template>
  <section>
    <h1>Совершите обмен за 3 шага</h1>
    <figure class="image-step-zero"></figure>
  </section>
  <section>
    <div class="step">Шаг 1</div>
    <h1>Создай или найди сделку</h1>
    <p>
      Широкий спектр услуг по торговле и управлению цифровыми активами для удовлетворения
    </p>
    <figure class="image-step-one"></figure>
  </section>
  <section>
    <div class="step">Шаг 2</div>
    <h1>Безопасно переведи средства</h1>
    <p>
      Широкий спектр услуг по торговле и управлению цифровыми активами для удовлетворения
    </p>
    <figure class="image-step-two"></figure>
  </section>
  <section class="last-section">
    <div class="step">Шаг 3</div>
    <h1>Заверши обмен</h1>
    <p>
      Широкий спектр услуг по торговле и управлению цифровыми активами для удовлетворения
    </p>
    <button class="button-start-transfer">Начать обмен</button>
  </section>
</template>
<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  section {
    margin: 32px 16px 24px 16px;
  }
  .last-section {
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  h1 {
    font-size: 24px;
    font-weight: 700;
    line-height: 32px;
  }
  p {
    font-size: 14px;
    font-weight: 500;
    line-height: 20px;
    color: #6f767e;
  }
  figure {
    background-size: cover;
    background-position: center;
    height: 176px;
    margin-inline-start: 0;
    margin-inline-end: 0;
    max-width: 320px;
    margin: auto;
  }
  .step {
    font-size: 14px;
    font-weight: 700;
    line-height: 20px;
    padding: 4px 16px 4px 16px;
    width: fit-content;
    background-color: #dfd3f7;
    border-radius: 24px;
  }
  .image-step-zero {
    background-image: url("../assets/image-zer-step.svg");
  }
  .image-step-one {
    background-image: url("../assets/image-step-one.svg");
  }
  .image-step-two {
    background-image: url("../assets/image-second-step.svg");
  }
  .button-start-transfer {
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
}
</style>
