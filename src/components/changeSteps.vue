<template>
  <section class="page__steps steps">
    <div class="steps__wrapper _container">
      <section class="steps__header">
        <h2 class="_header-sections">Make an exchange in 3 steps</h2>
        <button class="button-blue">Start exchange</button>
      </section>
      <section class="steps__item">
        <figure class="image-step-zero"></figure>
        <div class="step">Step 1</div>
        <h3>Create or find a deal</h3>
        <p>A wide range of digital asset trading and management services</p>
      </section>
      <section class="steps__item">
        <figure class="image-step-one"></figure>
        <div class="step">Step 2</div>
        <h3>Transfer funds securely</h3>
        <p>A wide range of digital asset trading and management services</p>
      </section>
      <section class="steps__item">
        <figure class="image-step-two"></figure>
        <div class="step">Step 3</div>
        <h3>Complete the exchange</h3>
        <p>A wide range of digital asset trading and management services</p>
      </section>
      <button class="button-blue">Start exchange</button>
    </div>
  </section>
</template>
<style scoped>
.steps {
  padding: 120px 0;
  border-bottom: 2px solid rgba(207, 219, 213, 0.6);
}
.steps__wrapper {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.steps__header {
  flex: 0 1 100%;
  display: flex;
  margin-bottom: 48px;
  align-items: center;
  justify-content: space-between;
}
.steps__header > h2 {
  flex-basis: 450px;
}
.steps__items {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 24px;
}
.steps__item {
  flex: 0 1 30%;
}
.steps__item > *:not(:last-child) {
  margin-bottom: 24px;
}

figure {
  background-size: cover;
  background-position: center;
  height: 200px;
  margin-inline-start: 0;
  margin-inline-end: 0;
  margin: auto;
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

.steps__item > h3 {
  font-size: 24px;
  font-weight: 700;
  line-height: 32px;
}
.steps__item > p {
  font-size: 24px;
  font-weight: 500;
  line-height: 32px;
  color: #6f767e;
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
.steps__wrapper > button {
  display: none;
}
@media (max-width: 980px) {
  .steps__header {
    flex-wrap: wrap;
    flex: 0 1 48%;
  }
  .steps__header > h2 {
    margin-bottom: 32px;
  }
  .steps__items {
    flex-wrap: wrap;
  }
  .steps__item {
    flex: 0 1 48%;
  }
}
@media (max-width: 630px) {
  .steps {
    padding: 80px 0;
  }
  .steps__items {
    flex-direction: column;
  }
  .steps__item {
    flex: 0 1 100%;
  }
  .steps__header {
    flex-wrap: wrap;
    flex: 0 1 auto;
  }
  .steps__header > button {
    display: none;
  }
  .steps__wrapper > button {
    display: flex;
    margin: 32px 0;
    width: 100%;
  }
}
</style>
