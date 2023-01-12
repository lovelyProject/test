<template>
  <div class="v-carousel">
    <div class="v-carousel__counter">
      <span class="counter bold">{{ currentSlide + 1 }}/8</span>
    </div>
    <div class="v-carousel__content">
      <vCarouselItem
        v-for="(slide, index) in slides"
        :key="index"
        :slide="slide"
        :currentSlide="currentSlide"
        :index="index"
        :direction="direction"
      />
      <vCarouselControls
        @prevSlide="prevSlide"
        @nextSlide="nextSlide"
        :currentSlide="currentSlide"
      />
      <a href="#" class="v-carousel__btn"
        ><span>Искать промокод</span>
        <svg
          class="btn-arrow"
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
      </a>
    </div>
  </div>
</template>

<script>
import vCarouselItem from "@/components/carousel/v-carousel-item.vue";
import vCarouselControls from "@/components/carousel/v-carousel-controls.vue";
export default {
  components: {
    vCarouselItem,
    vCarouselControls,
  },
  props: ["slides"],
  data() {
    return {
      currentSlide: 0,
      direction: "",
    };
  },
  methods: {
    nextSlide() {
      this.currentSlide++;
      this.direction = "right";
    },
    prevSlide() {
      this.currentSlide--;
      this.direction = "left";
    },
  },
};
</script>

<style lang="sass">
.v-carousel
    margin: 0 auto
    max-width: 90rem
    position: relative
    overflow: hidden
    min-height: 50rem
    border: .1rem solid black
    &__counter
        position: absolute
        left: 49%
        width: 4rem
        height: 4rem
        background-color: #fff
        margin: 0 auto
        border-radius: 50%
        display: flex
        align-items: center
        justify-content: center
        box-shadow: 0 .5rem 2.6rem rgba(0, 0, 0, 0.1)
        margin-bottom: 2rem
        & .counter
            font-size: 1.5rem
    &__content
        margin-top: 5rem
        position: relative
        min-height: 50rem
    &__btn
        position: absolute
        left: 42%
        top: 88%
        display: inline-block
        background-color: #fff
        text-decoration: none
        color: #333333
        padding: 1.9rem 1.3rem
        box-shadow: 0 .5rem 2.6rem rgba(11, 75, 92, 0.0975713)
        border-radius: .8rem
        align-items: center
        z-index: 6
        &:hover
            background-color: rgba(0,0,0,.1)
        & span
            margin-right: .4rem
.btn-arrow
    width: 2.8rem
    height: .5rem
</style>
