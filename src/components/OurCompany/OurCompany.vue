<script>
import OurCompanyLogo from "./OurCompanyLogo.vue";
import OurCompanyInfo from "./OurCompanyInfo.vue";
export default {
  name: "OurCompany",
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
  background-color: #191935;
  padding-top: 150px;
  padding-bottom: 100px;
  .container {
    height: 100%;
    display: flex;
    justify-content: space-between;
  }
}
</style>
