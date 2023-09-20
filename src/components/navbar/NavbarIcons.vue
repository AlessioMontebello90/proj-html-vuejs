<script>
export default {
  name: "NavbarIcons",
  data() {
    return {
      ShoppingItems: 0,
    };
  },
};
</script>

<template>
  <div class="icons">
    <div class="circle">
      <a href="#"><img src="../../assets/img/image (1).svg" alt="Search" /></a>
    </div>
    <div class="circle">
      <a href="#"
        ><img src="../../assets/img/image (3).svg" alt="Buy" />
        <div class="shopping-list circle-small">{{ ShoppingItems }}</div></a
      >
    </div>
  </div>
</template>

<style scoped lang="scss">
@use "../../assets/scss/variables" as *;
@use "../../assets/scss/mixins" as *;
.icons {
  display: flex;
  .circle {
    @include center();
    @include round();
    margin: 0 5px;
    height: 40px;
    width: 40px;
    background-color: $white;
    border-radius: 50%;
    position: relative;
    a {
      @include center();
      .circle-small {
        @include center();
        @include round();
        position: absolute;
        top: -30%;
        right: -30%;
        height: 25px;
        width: 25px;
        background-color: $blue;
        color: $white;
        padding: 12px;
      }
      img {
        height: 20px;
        filter: invert(13%) sepia(8%) saturate(6028%) hue-rotate(207deg)
          brightness(91%) contrast(96%);
      }
    }
  }
}
</style>
