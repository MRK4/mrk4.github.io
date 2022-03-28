<template>
  <!-- BACKGROUND -->
  <div class="flex flex-row justify-between fixed bubbles">
      <img class="w-1/2 h-screen" src="@/assets/imgs/bubble1.svg" alt="">
      <img class="w-1/2 h-screen" src="@/assets/imgs/bubble2.svg" alt="">
  </div>

  <div class="transition-all duration-300 ease-in bg-transparent dark:bg-gray-900 dark:text-white sm:overflow-hidden py-28 px-6 sm:px-24 flex flex-col sm:flex-row sm:justify-center items-center sm:h-full sm:w-full">
      <BluePannel />
      <div class="sm:py-14 flex flex-col sm:flex-row justify-around w-full h-full">
        <div class="px-5 h-full flex flex-col justify-between">
          <AboutMe />
          <ProExperience class="py-8" />
        </div>
        <div class="px-5 h-full flex flex-col justify-between">
          <Portfolio class="py-8 sm:py-0 sm:hidden 2xl:block" />
          <Skills class="py-8 sm:py-0" />
        </div>
      </div>
  </div>

  <div class="hidden sm:block text-sm dark:text-white text-center absolute py-1 h-fit w-full bottom-1 opacity-25">✨ Website made with VueJS & Tailwind - Code is available <a class="underline text-blue-400 hover:text-blue-200" href="https://github.com/MRK4/mrk4.github.io">here</a> ✨</div>

  <div class="bg-transparent dark:bg-gray-900 sm:hidden py-4 text-xs dark:text-white text-center w-full">✨ Website made with VueJS & Tailwind - <a class="underline text-blue-400 hover:text-blue-200" href="https://github.com/MRK4/mrk4.github.io">Code is available here</a> ✨</div>

  <div class="text-sm dark:text-white text-center absolute mt-4 h-fit w-full top-1">
    <div class="flex flex-row justify-center sm:space-x-2 align-items">
      <div class="label-light">🌞</div>
      <Toggler />
      <div class="label-dark opacity-25">🌙</div>
    </div>
  </div>

</template>

<script>
import BluePannel from './components/BluePannel.vue'
import AboutMe from './components/AboutMe.vue'
import ProExperience from './components/ProExperience.vue'
import Portfolio from './components/Portfolio.vue'
import Skills from './components/Skills.vue'
import Toggler from './components/Toggler.vue'

export default {
  name: 'App',
  components: {
    BluePannel,
    AboutMe,
    ProExperience,
    Portfolio,
    Skills,
    Toggler
  }
}

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Heebo:wght@400;700&display=swap');;

@font-face {
    font-family: 'Circular Std Book';
    src: url('./assets/fonts/CircularStd-Book.woff2') format('woff2'),
        url('./assets/fonts/CircularStd-Book.woff') format('woff');
    font-weight: 500;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'SF Pro Display';
    src: url('./assets/fonts/SFProDisplay-Regular.woff2') format('woff2'),
        url('./assets/fonts/SFProDisplay-Regular.woff') format('woff');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

@keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-moz-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-webkit-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-o-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

@-ms-keyframes fadeIn {
  0% {opacity:0;}
  100% {opacity:1;}
}

#app {
  margin: 0;
  padding: 0;
  height: 100vh;
  width: 100vw;
  color: #21243D;
  animation: fadeIn linear 1s;
  -webkit-animation: fadeIn linear 1s;
  -moz-animation: fadeIn linear 1s;
  -o-animation: fadeIn linear 1s;
  -ms-animation: fadeIn linear 1s;
}

.bubbles{
  z-index: -1;
}

.heebo{
  font-family: 'Heebo', sans-serif;
}

.circular-std-book{
  font-family: 'Circular Std Book', Arial, sans-serif;
}

.sf-pro-display-regular{
  font-family: 'SF Pro Display', Arial, sans-serif;
}

.category{
  text-decoration: underline;
  text-underline-offset: 6px;
}
</style>
