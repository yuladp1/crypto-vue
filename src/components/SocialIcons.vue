<template>
  <div class="page__icons-wrapper icons">
    <div class="icons__wrapper-scroll">
      <div class="icons__scroll"></div>
      <p class="icons__scroll-text">Scroll down</p>
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
</template>

<script>
export default {
  name: "socialIcons",
  created() {},
  data() {
    return {};
  },
  props: {},
  methods: {},
};
</script>

<style scoped>
.icons {
  padding: 47px 24px 24px 24px;
  background: #f5f9fe;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.icons__wrapper-scroll {
  display: flex;
  gap: 19px;
  align-items: center;
}
.icons__scroll {
  width: 18px;
  height: 18px;
  background: white;
  background: url("../assets/images/header-images/Vector.svg");
  background-position: center;
  background-size: 8px 8px;
  background-repeat: no-repeat;
  box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.04), 0px 8px 16px rgba(0, 0, 0, 0.08);
  border-radius: 9.35247px;
}

.icons__scroll-text {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 133%;
  color: #6f767e;
}

.icons__wrapper-content {
  display: flex;
  gap: 24px;
  align-items: center;
  justify-content: space-between;
}
.icons__wrapper-content > h2 {
  font-style: normal;
  font-weight: 500;
  font-size: 12px;
  line-height: 133%;
  color: #6f767e;
}
.icons__wrapper-icons {
  display: flex;
  gap: 16px;
  justify-content: flex-end;
}
.icons__wrapper-icons > div {
  width: 40px;
  height: 40px;
  background-position: center;
  background-repeat: no-repeat;
  box-shadow: 0px 0px 4px rgba(0, 0, 0, 0.04), 0px 8px 16px rgba(0, 0, 0, 0.08);
  border-radius: 50%;
}
.fb-icon {
  background: url("../assets/images/social-icons-images/fb.svg");
}
.twitter-icon {
  background: url("../assets/images/social-icons-images/twitter.svg");
}
.instagram-icon {
  background: url("../assets/images/social-icons-images/instagram.svg");
}
@media (max-width: 480px) {
  .icons {
    display: none;
  }
}
</style>
