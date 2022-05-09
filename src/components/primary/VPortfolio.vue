<template>
  <div class="flex jsutify-center items-center animate__animated animate__zoomIn animate__faster">
    <VNavbar />
  </div>
</template>

<script>
import VNavbar from "../seconds/VNavbar.vue";

export default {
  name: 'VPortfolio',
  components: {
    VNavbar
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input:checked ~ .dot {
  transform: translateX(100%);
}
</style>