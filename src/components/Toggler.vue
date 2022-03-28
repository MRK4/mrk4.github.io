<template>
    <div class="relative rounded-full inline-block w-10 mr-2 align-middle select-none transition duration-200 ease-in">
        <input type="checkbox" name="toggle" id="toggle" class="toggle toggle-checkbox absolute block w-6 h-6 rounded-full bg-white border-4 border-gray-400 dark:dark:border-gray-700 appearance-none cursor-pointer"/>
        <label for="toggle" class="toggle-label block overflow-hidden h-6 rounded-full bg-gray-400 dark:bg-gray-500 cursor-pointer"></label>
    </div>
</template>

<script>
export default {
  name: 'Toggler',
  mounted: function () {
    this.$nextTick(function () {
        const toggle = document.querySelector('.toggle');
        const html = document.querySelector('html');
        const labelLight = document.querySelector('.label-light');
        const labelDark = document.querySelector('.label-dark');

        toggle.onclick = function(){
            html.classList.toggle('dark');
            labelLight.classList.toggle('opacity-25');
            labelDark.classList.toggle('opacity-25');
        }
    })
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.toggle-checkbox:checked {
  right: 0;
  border-color: rgb(31, 41, 55);
}
.toggle-checkbox:checked + .toggle-label {
  background-color: rgb(31, 41, 55);
}

</style>