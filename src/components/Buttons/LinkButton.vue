<script>
export default {
  name: "LinkButton",
  props: {
    text: String,
  },
};
</script>

<template>
  <a class="read" href="#"
    ><b>{{ text }} More </b>
    <img
      class="img-fluid"
      src="../../assets/img/image (8).svg"
      alt="arrow-right"
  /></a>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
a.read {
  text-decoration: none;
  color: $darker-blue;
  background-color: $green;
  border-radius: 10px;
  padding: 15px 30px;
  margin: 0 20px;
  img {
    height: 18px;
  }
}
</style>
