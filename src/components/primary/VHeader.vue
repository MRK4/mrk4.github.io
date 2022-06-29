<template>
  <div class="flex flex-col items-center space-y-5 animate__animated animate__zoomIn animate__faster">
    <div class="h-44 w-44 rounded-full border-4 border-blue-500">
      <img class="h-full w-full rounded-full border-4 border-transparent shadow-xl shadow-blue-500/50 dark:shadow-blue-500/25" src="@/assets/img/photo.jpg" alt="Image de Clément Poudrée">
    </div>
    <div class="text-center">
      <h1 class="text-[#21243D] dark:text-white montserrat font-bold text-2xl">Clément Poudrée</h1>
      <h2 class="text-gris dark:text-gris hind font-normal text-base">Développeur Full-Stack</h2>
    </div>
    <div>
      <SocialMedias />
      <p class="mt-2 hind font-normal text-sm text-gris text-center">📍 Rennes, France</p>
    </div>
    <div>
      <LabelAccroche />
    </div>
    <div>
      <VButtons />
    </div>
  </div>
</template>

<script>
import SocialMedias from "../seconds/SocialMedias.vue";
import LabelAccroche from "../seconds/LabelAccroche.vue";
import VButtons from "../seconds/VButtons.vue";

export default {
  name: 'VHeader',
  components: {
    SocialMedias,
    LabelAccroche,
    VButtons
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
