<template>
  <div class="wrapper-sections-steps" id="how-work">
    <section class="wrapper-large-screen">
      <h1 class="h-medium-width">Make an exchange in 3 steps</h1>
      <button class="button-start-transfer-medium">Start exchange</button>
    </section>
    <div class="wrapper-steps">
      <section>
        <figure class="image-step-zero"></figure>
        <div class="step">Step 1</div>
        <h1>Create or find a deal</h1>
        <p>A wide range of digital asset trading and management services</p>
      </section>
      <section>
        <figure class="image-step-one"></figure>
        <div class="step">Step 2</div>
        <h1>Transfer funds securely</h1>
        <p>A wide range of digital asset trading and management services</p>
      </section>
      <section class="last-section">
        <figure class="image-step-two"></figure>
        <div class="step">Step 3</div>
        <h1>Complete the exchange</h1>
        <p>A wide range of digital asset trading and management services</p>
        <button class="button-start-transfer-mobile">Start exchange</button>
      </section>
    </div>
  </div>
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
  .button-start-transfer-medium {
    display: none;
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
  .button-start-transfer-mobile {
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

@media screen and (min-width: 721px) and (max-width: 1440px) {
  .wrapper-sections-steps {
    width: 100%;
    background-color: white;
    display: flex;
    flex-wrap: wrap;
    padding: 0 23.5px 64px 23.5px;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  section {
    width: 45%;
    margin: 32px 16px 24px 16px;
  }

  .h-medium-width {
    font-size: 48px;
    font-weight: 700;
    line-height: 56px;
  }
  .button-start-transfer-mobile {
    display: none;
  }
  .button-start-transfer-medium {
    margin-top: 32px;
    display: block;
    width: 169px;
    height: 56px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 18px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 32px 0 32px 0;
  }
  h1 {
    font-size: 24px;
    font-weight: 700;
    line-height: 32px;
  }
  p {
    font-size: 24px;
    font-weight: 500;
    line-height: 32px;
    color: #6f767e;
  }
  figure {
    background-size: cover;
    background-position: center;
    height: 200px;
    margin-inline-start: 0;
    margin-inline-end: 0;
    margin: auto;
  }
  .step {
    font-size: 16px;
    font-weight: 700;
    line-height: 24px;
    padding: 4px 16px;
    width: fit-content;
    background-color: #dfd3f7;
    border-radius: 24px;
    margin-top: 24px;
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

@media screen and (min-width: 1441px) {
  .wrapper-sections-steps {
    width: 100%;
    background-color: white;
    padding: 0 23.5px 64px 23.5px;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  .wrapper-large-screen {
    display: flex;
    padding: 120px 108px;
  }
  .wrapper-large-screen > h1 {
    flex-basis: 450px;
    font-size: 48px;
    line-height: 56px;
    margin-right: auto;
  }
  .wrapper-large-screen > button {
    flex-basis: 169px;
    height: 56px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 18px;
    font-weight: 500;
    color: white;
    display: block;
  }
  .button-start-transfer-mobile {
    display: none;
  }
  .wrapper-steps {
    display: flex;
    flex-wrap: nowrap;
    gap: 24px;
    padding: 48px 108px;
  }
  h1 {
    font-size: 24px;
    font-weight: 700;
    line-height: 32px;
  }
  p {
    font-size: 24px;
    font-weight: 500;
    line-height: 32px;
    color: #6f767e;
  }
  figure {
    background-size: cover;
    background-position: center;
    height: 200px;
    margin-inline-start: 0;
    margin-inline-end: 0;
    margin: auto;
  }
  .step {
    font-size: 16px;
    font-weight: 700;
    line-height: 24px;
    padding: 4px 16px;
    width: fit-content;
    background-color: #dfd3f7;
    border-radius: 24px;
    margin-top: 24px;
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
