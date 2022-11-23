<template>
  <footer>
    <p>© DEPO 2022</p>
    <div class="wrapper-terms-of-use">
      <a href="" class="terms">Terms of Use</a>
      <a href="">Privacy policy</a>
    </div>
    <h2>Our social networks</h2>
    <div class="wrapper-social-networks">
      <figure><img src="../assets/facebook.svg" alt="" /></figure>
      <figure><img src="../assets/twitter.svg" alt="" /></figure>
      <figure><img src="../assets/instagram.svg" alt="" /></figure>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  footer {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .wrapper-terms-of-use {
    display: flex;
    justify-content: center;
    margin: 24 auto 32 auto;
  }
  .wrapper-terms-of-use a {
    text-decoration: none;
    color: #6f767e;
  }
  .terms {
    margin-right: 32px;
  }
  h2,
  p,
  .wrapper-terms-of-use {
    font-size: 12px;
    font-weight: 500;
    line-height: 16px;
    color: #6f767e;
    margin-top: 24px;
    margin-bottom: 32px;
  }
  h2 {
    margin-bottom: 16px;
  }
  .wrapper-social-networks {
    width: 184px;
    display: flex;
    justify-content: space-between;
  }
  figure {
    width: 40px;
    height: 40px;
  }
  img {
    width: 100%;
    height: auto;
  }
}
@media screen and (min-width: 721px) and (max-width: 1440px) {
  footer {
    display: flex;
    align-items: center;
    padding-bottom: 24px;
    padding-left: 24px;
    background-color: white;
  }
  .wrapper-terms-of-use {
    display: flex;
    justify-content: center;
    margin: 0;
  }
  .wrapper-terms-of-use a {
    text-decoration: none;
    color: #6f767e;
  }
  .terms {
    padding-right: 24px;
  }
  h2,
  p,
  .wrapper-terms-of-use {
    font-size: 12px;
    font-weight: 500;
    line-height: 16px;
    color: #6f767e;
  }
  p {
    padding-right: 24px;
  }
  h2 {
    margin-right: 24px;
    margin-left: auto;
  }
  .wrapper-social-networks {
    width: 184px;
    display: flex;
    justify-content: space-between;
  }
  figure {
    width: 40px;
    height: 40px;
  }
  img {
    width: 100%;
    height: auto;
  }
}

@media screen and (min-width: 1441px) {
  footer {
    display: flex;
    align-items: center;
    background-color: white;
    width: 100%;
    padding-left: 108px;
  }
  .wrapper-terms-of-use {
    display: flex;
    justify-content: center;
    margin-left: auto;
    margin-right: 212px;
  }
  .wrapper-terms-of-use a {
    text-decoration: none;
    color: #6f767e;
  }
  .terms {
    padding-right: 24px;
  }
  h2,
  p,
  .wrapper-terms-of-use {
    font-size: 12px;
    font-weight: 500;
    line-height: 16px;
    color: #6f767e;
  }
  p {
    padding-right: 24px;
  }
  h2 {
    margin-right: 24px;
    margin-left: auto;
  }
  .wrapper-social-networks {
    width: 184px;
    display: flex;
    justify-content: space-between;
  }
  figure {
    width: 40px;
    height: 40px;
  }
  img {
    width: 100%;
    height: auto;
  }
}
</style>
