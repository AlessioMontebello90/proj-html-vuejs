<script>
import TestimonialsList from "./TestimonialsList.vue";
export default {
  name: "Testimonials",
  components: {
    TestimonialsList,
  },
};
</script>

<template>
  <div class="testimonials">
    <div class="container">
      <div class="title">
        <h5>testimonials</h5>
        <h3>What Our Client Say</h3>
      </div>
      <TestimonialsList />
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/mixins" as *;
@use "../../assets/scss/variables" as *;
.testimonials {
  height: 110vh;
  background-color: $darker-blue;
  padding: 150px 0;
}
.title {
  width: 40%;
  text-align: center;
  margin-bottom: 50px;
}
h5 {
  color: $dark-green;
}
h3 {
  color: $white;
  font-size: 40px;
}
</style>
93 changes: 93 additions & 0 deletions93
