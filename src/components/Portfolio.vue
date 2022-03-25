<template>

    <div>
        <div>
            <h2 class="category circular-std-book text-2xl">Projects</h2>
            <div class="mt-2 sf-pro-display-regular text-gray-500 dark:text-gray-400">Here's some work that I've made</div>
        </div>

        <div class="pt-7 circular-std-book text-center">

            <div class="grid grid-cols-3 gap-x-8 gap-y-10">
                <div class="flex flex-col h-44 w-60 rounded-3xl project-card">
                    <img class="transition-all duration-300 ease-in rounded-3xl h-full w-full shadow-lg border-2 border-gray-100 dark:border-gray-900 hover:border-blue-600 dark:hover:border-blue-400" src="@/assets/imgs/keskonfai.jpg" alt="Page d'accueil de Qu'est ce qu'on fait">
                    <div class="mt-2 text-gray-500 dark:text-gray-400">Keskonfai w/ BoredAPI</div>
                </div>
                <div class="flex flex-col h-44 w-60 rounded-3xl project-card">
                    <img class="transition-all duration-300 ease-in rounded-3xl h-full w-full shadow-lg border-2 border-gray-100 dark:border-gray-900 hover:border-blue-600 dark:hover:border-blue-400" src="@/assets/imgs/fireservice.jpg" alt="Page d'accueil de Fireservice.fr">
                    <div class="mt-2 text-gray-500 dark:text-gray-400">Fireservice</div>
                </div>
                <div class="flex flex-col h-44 w-60 rounded-3xl">
                    <div class="transition-all duration-300 ease-in rounded-3xl project-card h-full w-full bg-blue-200 dark:bg-gray-800 shadow-lg text-blue-600 dark:text-blue-400 border-2 border-gray-100 dark:border-gray-900 hover:border-blue-600 dark:hover:border-blue-400">Still working on...✍️</div>
                    <div class="mt-2 text-gray-500 dark:text-gray-400">Anim'Adopt</div>
                </div>
                <!-- <div class="flex flex-col h-44 w-60 rounded-3xl project-card border-dashed border-4 border-blue-200 bg-transparent text-blue-600">Maybe one day this box <br>will not be empty anymore 🤔</div>
                <div class="flex flex-col h-44 w-60 rounded-3xl project-card border-dashed border-4 border-blue-200 bg-transparent text-blue-600">Maybe one day this box <br>will not be empty anymore 🤔</div>
                <div class="flex flex-col h-44 w-60 rounded-3xl project-card border-dashed border-4 border-blue-200 bg-transparent text-blue-600">Maybe one day this box <br>will not be empty anymore 🤔</div> -->
            </div>

        </div>

    </div>

</template>

<script>
export default {
  name: 'Portfolio'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.project-card{
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
