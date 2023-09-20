<script>
import ButtonComposition from "../ButtonComposition.vue";
export default {
  name: "OurCompanyInfo",
  data() {
    return {
      text: "Discover",
    };
  },
  components: {
    ButtonComposition,
  },
};
</script>

<template>
  <div class="company-info">
    <h5>12 Years Experience</h5>
    <h3>We Are The Best Gaming Company</h3>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptas fugit
      maxime, hic dicta exercitationem sed adipisci ad quia molestias nemo
      dolores fugiat perspiciatis laboriosam incidunt numquam commodi sit,
      consequuntur distinctio.
    </p>
    <p>
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptas fugit
      maxime, hic dicta exercitationem sed adipisci ad quia molestias nemo
    </p>
    <ul class="p-0 mt-2">
      <li>
        <span class="round-border">
          <img src="../../assets/img/image (10).svg" alt="check" />
        </span>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate
      </li>
      <li>
        <span class="round-border">
          <img src="../../assets/img/image (10).svg" alt="check" />
        </span>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate
      </li>
      <li>
        <span class="round-border">
          <img src="../../assets/img/image (10).svg" alt="check" />
        </span>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate
      </li>
      <li>
        <span class="round-border">
          <img src="../../assets/img/image (10).svg" alt="check" />
        </span>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate
      </li>
    </ul>
    <ButtonComposition :text="text" />
  </div>
</template>

<style scoped lang="scss">
.company-info {
  flex-basis: 50%;
  padding-top: 20px;
  h5 {
    color: #05cc7c;
    margin-bottom: 20px;
  }
  h3 {
    color: white;
    margin-bottom: 35px;
    font-size: 50px;
  }
  p {
    color: white;
    margin-bottom: 20px;
  }
  li {
    list-style-type: none;
    color: white;
    display: flex;
    align-items: center;
    margin: 15px 0;
    span {
      width: 25px;
      height: 25px;
      border: 2px solid #05cc7c;
      border-radius: 50%;
      padding: 5px;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-right: 15px;
    }
    img {
      height: 15px;
      filter: invert(58%) sepia(70%) saturate(3143%) hue-rotate(118deg)
        brightness(102%) contrast(96%);
    }
  }
}
</style>
