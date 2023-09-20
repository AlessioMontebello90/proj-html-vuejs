<script>
export default {
  name: "PlayerIcons",
};
</script>

<template>
  <section class="player-icons">
    <figure>
      <img class="img-fluid" src="../../assets/img/t1.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t2.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t3.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t4.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t5.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t6.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t7.png" alt="ninja" />
    </figure>
    <figure>
      <img class="img-fluid" src="../../assets/img/t8.png" alt="ninja" />
    </figure>
  </section>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.player-icons {
  @include center("c-between");
  background-color: $darker-blue;
  border-radius: 25px;
  padding: 20px;
  margin: 50px 0;
  figure {
    @include center("cross");
    margin: 10px 0;
    img {
      height: 100px;
    }
  }
}
</style>
