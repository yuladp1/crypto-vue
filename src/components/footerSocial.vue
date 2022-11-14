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
</style>
