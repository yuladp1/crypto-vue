<template>
  <section class="lead-platform" id="about">
    <h1>Leading digital asset trading platform</h1>
    <article>
      A wide range of digital asset trading and management services to meet variety of
      trading needs. Comprehensive protection of user assets with our offline storage,
      multi-factor encryption and 24/7 security monitoring.
    </article>
  </section>
</template>
<style scoped>
@media screen and (min-width: 320px) and (max-width: 720px) {
  .lead-platform {
    margin: 32px 16px 0 16px;
    width: auto;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
  }
  h1 {
    font-size: 24px;
    font-weight: 700;
    line-height: 32px;
  }
  article {
    margin-top: 16px;
    padding-bottom: 32px;
    font-size: 14px;
    font-weight: 500;
    line-height: 24px;
  }
}
@media screen and (min-width: 721px) and (max-width: 1440px) {
  .lead-platform {
    width: 100%;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
    background-color: white;
    padding-left: 24px;
    padding-top: 80px;
  }
  h1 {
    width: 70%;
    font-size: 48px;
    font-weight: 700;
    line-height: 56px;
  }
  article {
    width: 70%;
    margin-top: 32px;
    padding-bottom: 80px;
    font-size: 18px;
    font-weight: 500;
    line-height: 32px;
  }
}

@media screen and (min-width: 1441px) {
  .lead-platform {
    display: flex;
    gap: 174px;
    border-bottom: 2px solid rgba(207, 219, 213, 0.6);
    background-color: white;
    padding: 120px 108px;
  }
  h1 {
    font-size: 48px;
    font-weight: 700;
    line-height: 56px;
    flex-basis: 550px;
    flex-grow: 1;
  }
  article {
    font-size: 18px;
    font-weight: 500;
    line-height: 32px;
    flex-basis: 550px;
    flex-grow: 1;
  }
}
</style>
