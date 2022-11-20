<template>
  <section>
    <p class="title-change-crypto">Обменивай крипту и фиат без ограничений</p>
    <button>Launch App</button>
    <div class="wrapper-icon-and-working-smart">
      <figure class="icon-copy"></figure>
      <p class="working-smart">Работает на смарт-контрактах</p>
    </div>
  </section>
</template>

<script>
export default {
  name: "launchApp",
  data() {},
  methods: {},
};
</script>
<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  section {
    background: #f5f9fe;
  }
  .title-change-crypto {
    padding: 32px 16px 24px 16px;
    color: black;
    font-family: "TT Firs Neue";
    font-weight: 700;
    font-style: normal;
    font-size: 32px;
    line-height: 40px;
    text-align: center;
    margin-block-start: 0;
    margin-block-end: 0;
  }
  button {
    width: 135px;
    height: 46px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 16px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 24px auto;
  }
  .wrapper-icon-and-working-smart {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 88px;
  }
  .icon-copy {
    background-image: url("../assets/ClipboardText.svg");
    width: 20px;
    height: 20px;
    margin-right: 5px;
    margin-inline-start: 0px;
  }
  .working-smart {
    font-size: 14px;
    font-weight: 500;
    color: #6f767e;
  }
}
@media screen and (min-width: 721px) {
  section {
    background: #f5f9fe;
  }
  .title-change-crypto {
    padding: 60px 60px 32px 60px;
    color: black;
    font-family: "TT Firs Neue";
    font-weight: 700;
    font-style: normal;
    font-size: 48px;
    line-height: 56px;
    text-align: center;
    margin-block-start: 0;
    margin-block-end: 0;
  }
  button {
    width: 159px;
    height: 64px;
    border-radius: 8px;
    border: 1px solid #3e8bf3;
    background-color: #3e8bf3;
    font-size: 20px;
    font-weight: 500;
    color: white;
    display: block;
    margin: 24px auto;
  }
  .wrapper-icon-and-working-smart {
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 60px;
  }
  .icon-copy {
    background-image: url("../assets/ClipboardText.svg");
    width: 24px;
    height: 24px;
    margin-right: 8px;
    margin-inline-start: 0px;
  }
  .working-smart {
    font-size: 16px;
    line-height: 24px;
    font-weight: 500;
    color: #6f767e;
  }
}
</style>
