<script>
import OurCompanyLogo from "./OurCompany/OurCompanyLogo.vue";
import OurCompanyInfo from "./OurCompany/OurCompanyInfo.vue";
export default {
  name: "AppMain",
  components: {
    OurCompanyLogo,
    OurCompanyInfo,
  },
};
</script>

<template>
  <section class="our-company">
    <div class="container">
      <OurCompanyLogo />
      <OurCompanyInfo />
    </div>
  </section>
</template>

<style scoped lang="scss">
.our-company {
  height: 100vh;
  background-color: #191935;
  padding-top: 150px;
  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
  }
}
</style>
