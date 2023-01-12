<template>
  <div class="main-wrapper">
    <div class="wrapper">
      <header class="header">
        <div class="header__burger">
          <svg
            viewBox="0 0 22 17"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M1.47498 0.528625V0.0286255H0.974976V0.528625H1.47498ZM21.0958 0.528625H21.5958V0.0286255H21.0958V0.528625ZM21.0958 2.52863V3.02863H21.5958V2.52863H21.0958ZM1.47498 2.52863H0.974976V3.02863H1.47498V2.52863ZM1.47498 7.70923V7.20923H0.974976V7.70923H1.47498ZM21.0958 7.70923H21.5958V7.20923H21.0958V7.70923ZM21.0958 9.70923V10.2092H21.5958V9.70923H21.0958ZM1.47498 9.70923H0.974976V10.2092H1.47498V9.70923ZM1.47498 14.5V14H0.974976V14.5H1.47498ZM1.47498 16.5H0.974976V17H1.47498V16.5ZM21.0958 16.5V17H21.5958V16.5H21.0958ZM21.0958 14.5H21.5958V14H21.0958V14.5ZM1.97498 0.0286255H1.47498V1.02863H1.97498V0.0286255ZM20.5958 0.0286255H1.97498V1.02863H20.5958V0.0286255ZM21.0958 0.0286255H20.5958V1.02863H21.0958V0.0286255ZM21.5958 1.02863V0.528625H20.5958V1.02863H21.5958ZM21.5958 2.02863V1.02863H20.5958V2.02863H21.5958ZM21.5958 2.52863V2.02863H20.5958V2.52863H21.5958ZM20.5958 3.02863H21.0958V2.02863H20.5958V3.02863ZM1.97498 3.02863H20.5958V2.02863H1.97498V3.02863ZM1.47498 3.02863H1.97498V2.02863H1.47498V3.02863ZM0.974976 2.02863V2.52863H1.97498V2.02863H0.974976ZM0.974976 1.02863V2.02863H1.97498V1.02863H0.974976ZM0.974976 0.528625V1.02863H1.97498V0.528625H0.974976ZM1.97498 7.20923H1.47498V8.20923H1.97498V7.20923ZM20.5958 7.20923H1.97498V8.20923H20.5958V7.20923ZM21.0958 7.20923H20.5958V8.20923H21.0958V7.20923ZM21.5958 8.20923V7.70923H20.5958V8.20923H21.5958ZM21.5958 9.20923V8.20923H20.5958V9.20923H21.5958ZM21.5958 9.70923V9.20923H20.5958V9.70923H21.5958ZM20.5958 10.2092H21.0958V9.20923H20.5958V10.2092ZM1.97498 10.2092H20.5958V9.20923H1.97498V10.2092ZM1.47498 10.2092H1.97498V9.20923H1.47498V10.2092ZM0.974976 9.20923V9.70923H1.97498V9.20923H0.974976ZM0.974976 8.20923V9.20923H1.97498V8.20923H0.974976ZM0.974976 7.70923V8.20923H1.97498V7.70923H0.974976ZM1.47498 15H1.97498V14H1.47498V15ZM1.97498 15V14.5H0.974976V15H1.97498ZM1.97498 16V15H0.974976V16H1.97498ZM1.97498 16.5V16H0.974976V16.5H1.97498ZM1.97498 16H1.47498V17H1.97498V16ZM20.5958 16H1.97498V17H20.5958V16ZM21.0958 16H20.5958V17H21.0958V16ZM20.5958 16V16.5H21.5958V16H20.5958ZM20.5958 15V16H21.5958V15H20.5958ZM20.5958 14.5V15H21.5958V14.5H20.5958ZM20.5958 15H21.0958V14H20.5958V15ZM1.97498 15H20.5958V14H1.97498V15Z"
              fill="#333333"
            />
          </svg>
        </div>
        <nav class="header__vertical-menu">
          <ul class="vertical-menu-list">
            <li class="vertical-menu-list__item">&nbsp;</li>
            <li class="vertical-menu-list__item">&nbsp;</li>
            <li class="vertical-menu-list__item">
              <span class="bold">03</span>&nbsp;&nbsp;&nbsp;&nbsp;Подсказки
            </li>
            <li class="vertical-menu-list__item">&nbsp;</li>
          </ul>
        </nav>
        <div class="header__info">
          <span>Листайте вниз</span>
          <svg
            viewBox="0 0 6 64"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path d="M3.03528 0.5V62.635" stroke="#333333" />
            <path
              d="M1.34137 60.9189L3.06208 62.6397L4.75292 60.9189"
              stroke="#333333"
            />
          </svg>
        </div>
      </header>
      <main class="main">
        <div class="main__logo">
          <img
            class="main__logo-item"
            src="@/assets/image/logo.png"
            alt="cloud"
          />
          <img
            src="@/assets/image/cloud-top-left.png"
            class="main__item cloud cloud-top-left"
            alt=""
          />
        </div>
        <div class="main__content">
          <img
            src="@/assets/image/cloud-middle-right.png"
            alt="cloud"
            class="main__item cloud cloud-middle-left"
          />
          <h1 class="main__title">ОНИ ДОЛЖНЫ ЧТО-ТО ЗНАТЬ</h1>
          <Carousel :slides="slides" />
          <img
            src="@/assets/image/cloud-bottom-left.png"
            class="cloud-bottom-left cloud"
            alt="cloud"
          />
          <img
            src="@/assets/image/cloud-bottom-left.png"
            class="cloud-bottom-left-2 cloud"
            alt="cloud"
          />
          <img
            src="@/assets/image/cloud-bottom-middle.png"
            class="cloud cloud-bottom-middle"
            alt="cloud"
          />
          <img
            src="@/assets/image/cloud-bottom-right.png"
            class="cloud cloud-bottom-right"
            alt="cloud"
          />
          <img
            src="@/assets/image/cloud-bottom-right.png"
            class="cloud cloud-bottom-right-2"
            alt="cloud"
          />
        </div>
      </main>
      <footer class="footer">
        <div class="footer-container">
          <span class="footer__link">hd.kinopoisk.ru</span>
        </div>
      </footer>
    </div>
  </div>
</template>
<script>
import Carousel from "./components/carousel/v-carousel.vue";

export default {
  name: "vApp",
  components: {
    Carousel,
  },
  data() {
    return {
      slides: [
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо2.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо3.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо4.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо5.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо6.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо7.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
        {
          image: "racer.png",
          text: "Для примера мы показали вам его лицо.  В первой серии он прячется в подвале за мониторами, и пусть борода не собьёт вас с толку. Найдите героя и нажмите  на паузу — ему не терпится отдать вам промокод.",
        },
      ],
    };
  },
};
</script>
<style lang="sass">
html
  font-size: 201%
*, ::after, ::before
  margin: 0
  padding: 0
  font-size: 1.6rem
  box-sizing: border-box
  text-decoration: none
  list-style: none
  color: #000
.main-wrapper
  background: url("@/assets/image/header-bg.jpg") center / cover no-repeat
  min-height: 100vh
.wrapper
  margin: 0 auto
  padding: 2rem 0 0 3.4rem
  position: relative
  min-height: 100vh
  overflow: hidden
.header
  display: flex
  flex-direction: column
  justify-content: space-between
  position: fixed
  height: 100vh
  &__vertical-menu
    max-width: 15.2rem
    font-size: 1.4rem
  &__info
    display: flex
    flex-direction: column
    align-items: center
    width: 2.1rem
    margin-left: -1rem
    margin-bottom: 3rem
    font-size: 2rem
    & svg
      display: block
      height: 6.4rem
      padding-top: 1rem
    & span
      display: block
      font-size: 1.4rem
      writing-mode: vertical-rl
      transform: rotate(180deg)
  &__slider
    width: 12.2rem
    height: 16.1rem
    & img
      width: 100%
  &__burger
    width: 2rem
    height: 1.6rem
    cursor: pointer
.main
  text-align: center
  display: flex
  flex-direction: column
  justify-content: space-between
  min-height: 100vh
  &__content
    position: relative
    overflow: hidden
  &__logo
    position: relative
    &-item
      width: 18.2rem
      margin-bottom: 2.4rem
  &__title
    font-weight: 700
    font-size: 4.5rem
    line-height: 7.2rem
    text-transform: uppercase
    color: #FFCC64
    margin-bottom: 3.4rem
.footer
  position: fixed
  top: 50%
  right: 0
  margin-right: 3rem
  z-index: 6
  &-container
  &__link
    writing-mode: vertical-lr
    transform: rotate(0deg)
.vertical-menu-list__item
  min-width: .8rem
  position: relative
  margin-bottom: 5rem
  text-decoration: underline
  text-underline-offset: .7rem
  font-size: 2rem
.bold
  font-weight: bold
.cloud
  position: absolute
  top: 0
  left: 0
  z-index: 0
  width: 50rem
  &-bottom
    &-left
      top: 43%
      &-2
        width: 60rem
        top: 10%
        left: 10%
    &-middle
      top: 64%
      left: 15%
    &-right
      top: 52%
      left: 33%
      &-2
        top: 52%
        left: 60%
  &-top-left
    left: 25rem
  &-middle-left
    top: 10%
    left: 75rem
@media (max-width: 3800px)
  html
    font-size: 200%
@media (max-width: 3200px)
  html
    font-size: 150%
@media (max-width: 2600px)
  html
    font-size: 130%
@media (max-width: 2200px)
  html
    font-size: 100%
@media (max-width: 1900px)
  html
    font-size: 90%
@media (max-width: 1712px)
  html
    font-size: 85%
@media (max-width: 1621px)
  html
    font-size: 75%
@media (max-width: 1422px)
  html
    font-size: 63%
@media (max-width: 1200px)
  html
    font-size: 60%
@media (max-width: 1140px)
  html
    font-size: 55%
@media (max-width: 1050px)
  html
    font-size: 50%
@media (max-width: 950px)
  html
    font-size: 45%
</style>
