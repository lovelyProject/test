<template>
  <div class="carousel">
    <div class="carousel__counter">1/8</div>
    <div class="carousel-inner">
      <vCarouselItem
        v-for="(slide, index) in slides"
        :key="index"
        :slide="slide"
        :current-slide="currentSlide"
        :index="index"
      />
      <!-- <a class="carousel__btn">
        <span>Искать промокод</span>
        <svg
          width="28"
          height="5"
          viewBox="0 0 28 5"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path d="M0.370911 2.8553L26.7406 2.8553" stroke="#333333" />
          <path
            d="M25.0246 4.54921L26.7453 2.8285L25.0246 1.13766"
            stroke="#333333"
          />
        </svg>
      </a> -->
      <vCarouselControls />
    </div>
  </div>
</template>

<script>
import vCarouselItem from "@/components/v-carousel-item.vue";
import vCarouselControls from "@/components/v-carousel-controls.vue";
export default {
  components: {
    vCarouselItem,
    vCarouselControls,
  },
  props: ["slides"],
  data() {
    return {
      currentSlide: 0,
    };
  },
};
</script>

<style lang="sass">
.carousel
    max-width: 90rem
    margin: 0 auto
    &__counter
        width: 5.6rem
        height: 5.6rem
        background-color: #fff
        border-radius: 50%
        text-align: center
        display: flex
        flex-direction: column
        justify-content: center
        margin: 0 auto 1.5rem auto
        box-shadow: 0 .5rem 2.6rem rgba(0, 0, 0, 0.1)
        font-size: 1.5rem
        line-height: 1.8rem
    &-inner
        display: flex
        justify-content: center
        flex-wrap: wrap
        position: relative
        width: 90rem
        padding-top: 32rem
        margin-top: 21.4rem
    &__btn
        padding: 1.9rem 2.7rem 1.9rem 1.3rem
        background-color: #fff
.carousel__button
    width: 4rem
    height: 4rem
    border: .1rem solid black
    background-color: #fff
    border-radius: 50%
    text-align: center
    display: flex
    flex-direction: column
    justify-content: center
.next-slide
    top: 50%
    right: 0
</style>
