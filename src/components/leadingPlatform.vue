<template>
  <section class="page__lead-platform lead-platform">
    <div class="platform__wrapper _container">
      <h1 class="_header-sections">Leading digital asset trading platform</h1>
      <article>
        A wide range of digital asset trading and management services to meet variety of
        trading needs. Comprehensive protection of user assets with our offline storage,
        multi-factor encryption and 24/7 security monitoring.
      </article>
    </div>
  </section>
</template>
<style scoped>
.lead-platform {
  padding: 130px 15px;
  border-bottom: 1px solid #d9d9d9;
}
.platform__wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
h1 {
  flex-basis: 554px;
}
article {
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 178%;
  color: #6f767e;
  flex-basis: 496px;
}
@media (max-width: 980px) {
  .platform__wrapper {
    flex-direction: column;
  }
  .lead-platform {
    padding: 80px 0;
  }
  h1 {
    margin-bottom: 32px;
    flex: 0 1 80%;
  }
  article {
    flex: 0 1 80%;
  }
}
@media (max-width: 400px) {
  .platform__wrapper {
    padding: 30px 15px;
  }
  h1 {
    flex: 0 1 100%;
  }
  article {
    flex: 0 1 100%;
    font-size: 16px;
  }
}
</style>
