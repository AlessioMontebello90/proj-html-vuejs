<script>
export default {
  name: "ButtonComposition",
  props: {
    text: String,
  },
};
</script>

<template>
  <div class="buttons justify-content-center">
    <a class="read" href="#"
      ><b>{{ text }} More </b>
      <img
        class="img-fluid"
        src="../assets/img/image (8).svg"
        alt="arrow-right"
    /></a>
    <a class="arrow" href="#">
      <img
        class="img-fluid"
        src="../assets/img/image (9).svg"
        alt="arrow-right"
    /></a>
  </div>
</template>

<style scoped lang="scss">
.buttons {
  display: flex;
  align-items: center;
  justify-content: center;
  a.read {
    text-decoration: none;
    color: #202046;
    background-color: #05cc7c;
    border-radius: 10px;
    padding: 15px 30px;
    margin: 0 20px;
    img {
      height: 18px;
    }
  }
  a.arrow {
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    color: #202046;
    background-color: #05cc7c;
    border-radius: 50%;
    padding: 20px 22px;
    img {
      height: 20px;
    }
  }
}
</style>
