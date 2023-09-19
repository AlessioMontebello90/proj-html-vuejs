<script>
export default {
  name: "HeaderJumbo",
};
</script>

<template>
  <div class="welcome">
    <h5>WELCOME TO RAXG</h5>
    <h1>ARE YOU READY FOR YOUR NEXT CHALLENGE?</h1>
    <div class="buttons">
      <a class="read" href="#"
        ><b>Read More </b>
        <img
          class="img-fluid"
          src="../../assets/img/image (8).svg"
          alt="arrow-right"
      /></a>
      <a class="arrow" href="#">
        <img
          class="img-fluid"
          src="../../assets/img/image (9).svg"
          alt="arrow-right"
      /></a>
    </div>
  </div>
</template>

<style scoped lang="scss">
.welcome {
  text-align: center;
  h5 {
    color: #05cc7c;
    margin-bottom: 20px;
  }
  h1 {
    color: white;
    font-size: 70px;
    margin-bottom: 50px;
  }
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
}
</style>
