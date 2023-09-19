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
.icons {
  display: flex;
  .circle {
    margin: 0 5px;
    height: 40px;
    width: 40px;
    background-color: white;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    a {
      display: flex;
      align-items: center;
      justify-content: center;
      .circle-small {
        position: absolute;
        top: -30%;
        right: -30%;
        height: 25px;
        width: 25px;
        border-radius: 50%;
        background-color: #4350ff;
        color: white;
        display: flex;
        align-items: center;
        justify-content: center;
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
