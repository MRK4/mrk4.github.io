<template>
  <div class="flex flex-col justify-around px-6 pb-8 sm:py-14 h-fit w-fit rounded-2xl bg-transparent text-sm">

    <div class="">
      <img class="h-auto w-48 rounded-full ombre border-2 border-blue-600 dark:border-blue-400" src="@/assets/imgs/avatar.png" alt="">

      <div class="pt-8 sf-pro-display-regular text-xs text-blue-600 dark:text-blue-400 space-y-4 sm:space-y-0">
        <div>
          <a class="transition-all duration-150 ease-in flex flex-row items-center underline text-blue-600 dark:text-blue-400 hover:text-blue-200" href="mailto:poudree.clement@gmail.com">
            <div><i class="fa-solid fa-envelope h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">poudree.clement@gmail.com</div>
          </a>
        </div>
        <div>
          <a class="transition-all duration-150 ease-in py-2 flex flex-row items-center underline text-blue-600 dark:text-blue-400 hover:text-blue-200" href="https://www.linkedin.com/in/clementpdr/">
            <div><i class="fa-brands fa-linkedin h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">LinkedIn</div>
          </a>
        </div>
        <div>
          <a class="transition-all duration-150 ease-in pb-2 flex flex-row items-center underline text-blue-600 dark:text-blue-400 hover:text-blue-200" href="https://github.com/MRK4">
            <div><i class="fa-brands fa-github h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">Github</div>
          </a>
        </div>
        <div>
          <a class="transition-all duration-150 ease-in flex flex-row items-center underline text-blue-600 dark:text-blue-400 hover:text-blue-200" href="https://www.google.com/maps/place/Rennes">
            <div><i class="fa-solid fa-location-dot h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">Rennes, France</div>
          </a>
        </div>
      </div>
    </div>

    <div class="pt-8 flex flex-col text-center justify-center circular-std-book space-y-4">

      <div class="pb-4 category text-xl">Education</div>

      <div class="flex flex-col justify-center">
        <!-- <img class="h-7" src="@/assets/imgs/diamond.svg" alt="Just a little fancy diamond"> -->
        <div><i class=" fa-solid fa-graduation-cap fa-xl text-blue-600 dark:text-blue-400"></i></div>
        <div class="py-2">Three-Year University</div>
        <div class="sf-pro-display-regular">Sep 2021 - Jul 2022</div>
      </div>

      <div class="py-6 flex flex-col justify-center">
        <!-- <img class="h-7" src="@/assets/imgs/diamond.svg" alt="Just a little fancy diamond"> -->
        <div><i class=" fa-solid fa-graduation-cap fa-xl text-blue-600 dark:text-blue-400"></i></div>
        <div class="py-2">Two-Year Technical</div>
        <div class="sf-pro-display-regular">Sep 2019 - Jul 2021</div>
      </div>

      <div class="flex flex-col justify-center">
        <!-- <img class="h-7" src="@/assets/imgs/diamond.svg" alt="Just a little fancy diamond"> -->
        <div><i class=" fa-solid fa-graduation-cap fa-xl text-blue-600 dark:text-blue-400"></i></div>
        <div class="py-2">High-School</div>
        <div class="sf-pro-display-regular">Sep 2016 - Jul 2019</div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'BluePannel'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.ombre{
  filter: drop-shadow(0px 10px 10px rgba(36, 36, 77, 0.25));
}
</style>
