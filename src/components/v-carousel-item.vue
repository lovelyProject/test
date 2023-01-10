<template>
  <div class="carousel-item" v-show="currentSlide === index">
    <img class="carousel-item__photo" src="@/assets/slides/racer.png" alt="" />
    <p class="carousel-item__description">{{ slide.text }}</p>
  </div>
</template>

<script>
export default {
  props: ["slide", "currentSlide", "index"],
};
</script>

<style lang="sass">
.carousel-item
  text-align: center
  position: absolute
  top: 0
  left: 0
  &__photo
  &__description
    max-width: 90rem
    font-size: 2rem
</style>
