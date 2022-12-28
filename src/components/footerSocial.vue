<template>
  <footer class="page__footer footer" id="contacts">
    <div class="footer__wrapper _container">
      <p>© DEPO 2022</p>
      <div class="footer__terms">
        <a href="">Terms of Use</a>
        <a href="">Privacy policy</a>
      </div>

      <div class="icons__wrapper-content">
        <h2>Our social networks</h2>
        <div class="icons__wrapper-icons">
          <div class="fb-icon"></div>
          <div class="twitter-icon"></div>
          <div class="instagram-icon"></div>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "footerSocial",
};
</script>
<style scoped>
.footer {
  padding: 76px 0;
}
.footer__wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.footer__terms {
  display: flex;
  gap: 32px;
  align-items: center;
}
.footer__terms a {
  text-decoration: none;
  color: #6f767e;
}
h2,
p,
.footer__terms {
  font-size: 12px;
  font-weight: 500;
  line-height: 16px;
  color: #6f767e;
}
@media (max-width: 600px) {
  .footer {
    padding: 30px 0;
  }
  .footer__wrapper {
    flex-direction: column;
    gap: 20px;
  }
  .icons__wrapper-content {
    flex-direction: column;
  }
}
</style>
