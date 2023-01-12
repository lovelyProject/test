<template>
  <button class="carousel-control prev-slide">Prev</button>
  <button class="carousel-control next-slide">
    <svg
      width="17"
      height="5"
      viewBox="0 0 17 5"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path d="M0.963876 2.38841L16.1642 2.38841" stroke="#333333" />
      <path
        d="M14.4482 4.08231L16.1689 2.3616L14.4482 0.670764"
        stroke="#333333"
      />
    </svg>
  </button>
</template>

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
    z-index: 20
    display: flex
    justify-content: center
    align-items: center
</style>
