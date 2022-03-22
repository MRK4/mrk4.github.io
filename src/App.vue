<template>
  <!-- BACKGROUND -->
  <div class="flex flex-row fixed bubbles">
      <img class="w-1/2 h-screen" src="@/assets/imgs/bubble1.svg" alt="">
      <img class="w-1/2 h-screen" src="@/assets/imgs/bubble2.svg" alt="">
  </div>

  <div class="select-none py-28 px-24 flex flex-row justify-center align-center conten-center items-center h-full w-full">
      <BluePannel />
      <div class="flex flex-row justify-around w-full h-full">
        <div class="px-5 h-full flex flex-col justify-around">
          <AboutMe />
          <ProExperience />
        </div>
        <div class="px-5 h-full flex flex-col justify-around">
          <Portfolio />
          <Skills />
        </div>
      </div>
  </div>

  <div class="text-center absolute py-1 h-fit w-full bottom-1 opacity-25">✨ Website made with VueJS - Code is available <a href="">here</a> ✨</div>
</template>

<script>
import BluePannel from './components/BluePannel.vue'
import AboutMe from './components/AboutMe.vue'
import ProExperience from './components/ProExperience.vue'
import Portfolio from './components/Portfolio.vue'
import Skills from './components/Skills.vue'

export default {
  name: 'App',
  components: {
    BluePannel,
    AboutMe,
    ProExperience,
    Portfolio,
    Skills
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

#app {
  margin: 0;
  padding: 0;
  height: 100vh;
  width: 100vw;
  color: #21243D;
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

#app a{
  color: #2F80ED;
  text-decoration: underline;
}

#app a:hover{
    color: #0054F7;
}
</style>
