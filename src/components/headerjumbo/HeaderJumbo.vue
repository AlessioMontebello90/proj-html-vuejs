<script>
import ButtonComposition from "../ButtonComposition.vue";
export default {
  name: "HeaderJumbo",
  components: {
    ButtonComposition,
  },
  data() {
    return {
      text: "Read",
    };
  },
};
</script>

<template>
  <div class="welcome">
    <h5>WELCOME TO RAXG</h5>
    <h1>ARE YOU READY FOR YOUR NEXT CHALLENGE?</h1>
    <ButtonComposition :text="text" />
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
.welcome {
  text-align: center;
  h5 {
    color: $dark-green;
    margin-bottom: 20px;
  }
  h1 {
    color: $white;
    font-size: 70px;
    margin-bottom: 50px;
  }
}
</style>
