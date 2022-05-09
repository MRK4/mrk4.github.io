<template>
  <div class="transition-all duration-150 ease-in bg-white dark:bg-gray-900 scroll-smooth px-14 pt-16 pb-4 flex flex-col items-center animate__animated">
    <div class="w-full flex flex-row justify-end">
      <div class="cursor-pointer p-2">
        <i class="toggle1 icon-light fa-regular fa-moon fa-lg text-blue-500 fill-current dark:text-blue-500 drop-shadow" alt="îcone de lune"></i>
        <i class="toggle2 icon-dark fa-solid fa-sun fa-lg text-[#21243D] fill-current dark:text-yellow-500 drop-shadow hidden" alt="îcone de soleil"></i>
      </div>
    </div>
    <div class="flex flex-col items-center space-y-6">
      <VHeader />
      <VPortfolio />
    </div>
    <VFooter />
  </div>
</template>

<script>
import VHeader from './components/primary/VHeader.vue'
import VPortfolio from './components/primary/VPortfolio.vue'
import VFooter from './components/primary/VFooter.vue'

export default {
  name: 'App',
  components: {
    VHeader,
    VPortfolio,
    VFooter
  },
  mounted: function () {
    this.$nextTick(function () {
      const toggle1 = document.querySelector('.toggle1');
      const toggle2 = document.querySelector('.toggle2');
      const html = document.querySelector('html');
      const iconLight = document.querySelector('.icon-light');
      const iconDark = document.querySelector('.icon-dark');
      toggle1.onclick = function(){
          html.classList.toggle('dark');
          iconLight.classList.toggle('hidden');
          iconDark.classList.toggle('hidden');
      }
      toggle2.onclick = function(){
          html.classList.toggle('dark');
          iconLight.classList.toggle('hidden');
          iconDark.classList.toggle('hidden');
      }
    })
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Hind&family=Montserrat:wght@400;500;600;700&display=swap');

#app{
  font-family: Hind, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: 0;
  padding: 0;
}

.montserrat{
  font-family: 'Montserrat', sans-serif;
}

.hind{
  font-family: 'Hind', sans-serif;
}

.text-gris{
  color: #86878C;
}

</style>
