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
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.our-company {
  background-color: $darkest-blue;
  padding-top: 150px;
  padding-bottom: 100px;
  .container {
    @include center("between");
    height: 100%;
  }
}
</style>
