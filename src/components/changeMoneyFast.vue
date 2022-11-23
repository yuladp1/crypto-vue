<template>
  <section>
    <div class="wrapper-large-text-and-button">
      <h1>Обменяйте средства за считанные минуты</h1>
      <p>
        Широкий спектр услуг по торговле и управлению цифровыми активами для
        удовлетворения
      </p>
      <button>Launch App</button>
    </div>
    <figure></figure>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  section {
    background-color: #f5f9fe;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  h1 {
    font-size: 24px;
    font-weight: 700;
    line-height: 32px;
    padding: 32px 16px 16px 16px;
    text-align: center;
  }
  p {
    font-size: 14px;
    font-weight: 500;
    line-height: 20px;
    color: #6f767e;
    text-align: center;
    padding: 0 16px;
  }
  button {
    width: 137px;
    height: 48px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 16px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 16px 0;
  }
  figure {
    width: 288px;
    height: 333px;
    background-image: url("../assets/image-mobile.svg");
  }
}

@media screen and (min-width: 721px) and (max-width: 1440px) {
  section {
    background-color: #f5f9fe;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  h1 {
    font-size: 48px;
    font-weight: 700;
    line-height: 56px;
    padding: 80px 90px 32px 80px;
    text-align: center;
  }
  p {
    font-size: 18px;
    font-weight: 500;
    line-height: 32px;
    color: #6f767e;
    text-align: center;
    padding: 0 115px 32px 115px;
  }
  button {
    width: 148px;
    height: 56px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 18px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 16px 0;
  }
  figure {
    width: 456px;
    height: 528px;
    background-image: url("../assets/image-mobile.svg");
    background-repeat: no-repeat;
    background-size: cover;
  }
}

@media screen and (min-width: 1441px) {
  section {
    background-color: #f5f9fe;
    width: 100%;
    height: 520px;
    display: flex;
    align-items: center;
    gap: 192px;
  }
  .wrapper-large-text-and-button {
    display: flex;
    flex-direction: column;
    flex-basis: 542px;
    flex-grow: 1;
    padding-left: 108px;
  }
  h1 {
    font-size: 48px;
    font-weight: 700;
    line-height: 56px;
  }
  p {
    font-size: 18px;
    font-weight: 500;
    line-height: 32px;
    color: #6f767e;
  }
  button {
    width: 148px;
    height: 56px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 18px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 16px 0;
  }
  figure {
    width: 505px;
    height: 600px;
    align-self: flex-end;
    overflow-y: visible;
    background-image: url("../assets/image-mobile.svg");
    background-repeat: no-repeat;
    background-size: cover;
  }
}
</style>
