<template>
  <a
    v-show="currentSlide != 0"
    class="carousel-control prev-slide"
    @click="prevSlide"
    ><svg viewBox="0 0 17 5" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M0.963876 2.38841L16.1642 2.38841" stroke="#333333" />
      <path
        d="M14.4482 4.08231L16.1689 2.3616L14.4482 0.670764"
        stroke="#333333"
      /></svg
  ></a>
  <a
    class="carousel-control next-slide"
    @click="nextSlide"
    v-show="currentSlide != 7"
  >
    <svg viewBox="0 0 17 5" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M0.963876 2.38841L16.1642 2.38841" stroke="#333333" />
      <path
        d="M14.4482 4.08231L16.1689 2.3616L14.4482 0.670764"
        stroke="#333333"
      />
    </svg>
  </a>
</template>

<script>
export default {
  methods: {
    prevSlide() {
      this.$emit("prevSlide", {});
    },
    nextSlide() {
      this.$emit("nextSlide", {});
    },
  },
  props: ["currentSlide"],
};
</script>
<style lang="sass">
.carousel-control
  border: .1rem solid rgba(51,51,51,1)
  border-radius: 50%
  width: 4rem
  height: 4rem
  display: inline-block
  position: absolute
  top: 0
  cursor: pointer
  z-index: 2
  display: flex
  justify-content: center
  align-items: center
  & svg
    width:1.7rem
    height:.5rem
  &:hover
    background-color: #fff
.prev-slide
  position: absolute
  top: calc(50% - 4rem)
  transform: rotate(180deg)
.next-slide
  position: absolute
  top: calc(50% - 4rem)
  right: 0
</style>
