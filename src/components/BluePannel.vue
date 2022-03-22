<template>
  <div class="flex flex-col justify-around px-6 py-14 h-full w-fit rounded-2xl bg-transparent border-4 border-blue-600 shadow-lg text-sm">

    <div class="">
      <img class="h-auto w-48 rounded-full ombre" src="@/assets/imgs/avatar.png" alt="">

      <div class="pt-8 sf-pro-display-regular text-xs text-blue-600">
        <div>
          <a class="flex flex-row items-center" href="mailto:poudree.clement@gmail.com">
            <div><i class="fa-solid fa-envelope h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">poudree.clement@gmail.com</div>
          </a>
        </div>
        <div>
          <a class="py-2 flex flex-row items-center" href="https://www.linkedin.com/in/clementpdr/">
            <div><i class="fa-brands fa-linkedin h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">LinkedIn</div>
          </a>
        </div>
        <div>
          <a class="pb-2 flex flex-row items-center" href="https://github.com/MRK4">
            <div><i class="fa-brands fa-github h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">Github</div>
          </a>
        </div>
        <div>
          <a class="flex flex-row items-center" href="https://www.google.com/maps/place/Rennes">
            <div><i class="fa-solid fa-location-dot h-3 w-3 fill-blue-500"></i></div>
            <div class="ml-2">Rennes, France</div>
          </a>
        </div>
      </div>
    </div>

    <div class="pt-8 flex flex-col text-center justify-center circular-std-book">

      <div class="pb-4 category text-xl">Education</div>

      <div class="flex flex-col justify-center">
        <img class="h-7" src="@/assets/imgs/diamond.svg" alt="Just a little fancy diamond">
        <div class="py-1">Three-Year University</div>
        <div class="sf-pro-display-regular">Sep 2021 - Jul 2022</div>
      </div>

      <div class="py-6 flex flex-col justify-center">
        <img class="h-7" src="@/assets/imgs/diamond.svg" alt="Just a little fancy diamond">
        <div class="py-1">Two-Year Technical</div>
        <div class="sf-pro-display-regular">Sep 2019 - Jul 2021</div>
      </div>

      <div class="flex flex-col justify-center">
        <img class="h-7" src="@/assets/imgs/diamond.svg" alt="Just a little fancy diamond">
        <div class="py-1">High-School</div>
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
