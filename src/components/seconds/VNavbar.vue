<template>
  <div class="flex flex-col w-full">
    <div class="flex justify-center">
      <ul class="w-72 p-2 flex flex-row rounded-xl bg-[#D0D0DA] dark:bg-gray-800 shadow-inner">
        <li class="flex-auto text-center">
          <a class="montserrat font-semibold text-base px-5 py-3 rounded-xl block leading-normal dark:text-white cursor-pointer" v-on:click="toggleTabs(1)" v-bind:class="{'bg-transparent': openTab !== 1, 'bg-white dark:bg-gray-900 shadow-lg': openTab === 1}">
            Projects
          </a>
        </li>
        <li class="flex-auto text-center">
          <a class="montserrat font-semibold text-base px-5 py-3 rounded-xl block leading-normal dark:text-white cursor-pointer" v-on:click="toggleTabs(2)" v-bind:class="{'bg-transparent': openTab !== 2, 'bg-white dark:bg-gray-900 shadow-lg': openTab === 2}">
            Skills
          </a>
        </li>
      </ul>
    </div>
    <div class="relative flex flex-col items-center min-w-0 break-words">
      <div class="py-5">
        <div class="flex justify-center tab-content tab-space">

          <!-- PROJECTS -->

          <div v-bind:class="{'hidden': openTab !== 1, 'block': openTab === 1}">
            <div class="max-w-6xl flex flex-wrap justify-center items-center space-x-0 sm:space-x-6">

                <!-- Price Components -->
                <div class="my-4 sm:max-w-md sm:max-h-72">
                  <a class="flex flex-col space-y-3 decoration-2 decoration-blue-500 hover:underline active:underline focus:underline" href="./price_component/index.html" target="_blank">
                    <img class="w-full h-auto rounded-xl shadow-xl border-2 border-gray-300 dark:border-gray-600 hover:border-blue-500 dark:hover:border-blue-500" src="@/assets/img/component_prices.png" alt="Capture d'écran représentant une page de composants de liste de prix">
                    <div class="flex flex-row justify-center items-end space-x-2">
                      <div class="montserrat font-bold text-xl text-[#21243D] dark:text-white">Prices Component</div>
                      <div class="hind font-normal text-base text-gris dark:text-gris">2022</div>
                    </div>
                  </a>
                </div>

                <!-- AdoptonCompagnon -->
                <div class="my-4 sm:max-w-md sm:max-h-72">
                  <a class="flex flex-col space-y-3 decoration-2 decoration-blue-500 hover:underline active:underline focus:underline" target="_blank">
                    <img class="w-full h-auto rounded-xl shadow-xl border-2 border-gray-300 dark:border-gray-600 hover:border-blue-500 dark:hover:border-blue-500" src="@/assets/img/workinprogress.jpg" alt="Capture d'écran représentant la page d'accueil d'Adopt'on Compagnon">
                    <div class="flex flex-row justify-center items-end space-x-2">
                      <div class="montserrat font-bold text-xl text-[#21243D] dark:text-white">Adopton-Compagnon</div>
                      <div class="hind font-normal text-base text-gris dark:text-gris">2022</div>
                    </div>
                  </a>
                </div>

                <!-- Whatwedo -->
                <div class="my-4 sm:max-w-md sm:max-h-72">
                  <a class="flex flex-col space-y-3 decoration-2 decoration-blue-500 hover:underline active:underline focus:underline" target="_blank">
                    <img class="w-full h-auto rounded-xl shadow-xl border-2 border-gray-300 dark:border-gray-600 hover:border-blue-500 dark:hover:border-blue-500" src="@/assets/img/keskonfai.jpg" alt="Capture d'écran représentant la page d'accueil de Keskonfai.fr">
                    <div class="flex flex-row justify-center items-end space-x-2">
                      <div class="montserrat font-bold text-xl text-[#21243D] dark:text-white">Interface BoredAPI</div>
                      <div class="hind font-normal text-base text-gris dark:text-gris">2022</div>
                    </div>
                  </a>
                </div>

                <!-- FIRESERVICE -->
                <div class="my-4 sm:max-w-md sm:max-h-72">
                  <a class="flex flex-col space-y-3 decoration-2 decoration-blue-500 hover:underline active:underline focus:underline" href="https://www.fireservice.fr" target="_blank">
                    <img class="w-full h-auto rounded-xl shadow-xl border-2 border-gray-300 dark:border-gray-600 hover:border-blue-500 dark:hover:border-blue-500" src="@/assets/img/fireservice.jpg" alt="Capture d'écran représentant la page d'accueil de Fireservice.fr">
                    <div class="flex flex-row justify-center items-end space-x-2">
                      <div class="montserrat font-bold text-xl text-[#21243D] dark:text-white">Fireservice</div>
                      <div class="hind font-normal text-base text-gris dark:text-gris">2020</div>
                    </div>
                  </a>
                </div>

            </div>
          </div>



          <!-- SKILLS -->

          <div v-bind:class="{'hidden': openTab !== 2, 'block': openTab === 2}">
            <div class="max-w-6xl flex flex-wrap flex-col sm:items-center space-y-9">

                <div class="sm:flex sm:flex-row sm:space-x-9">
                  <!-- FRONT-END -->
                  <div>
                    <div class="flex flex-col">
                      <div class="py-2 montserrat font-bold text-xl text-center text-[#21243D] dark:text-white">Front-End Development</div>
                      <div class="flex flex-row justify-between">

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>HTML</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>CSS</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>JavaScript</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>WordPress</div>
                          </div>
                        </div>

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>VueJS</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>TailwindCSS</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>Bootstrap</div>
                          </div>
                        </div>

                      </div>
                    </div>
                  </div>

                  <!-- BACK-END -->
                  <div>
                    <div class="flex flex-col">
                      <div class="py-2 montserrat font-bold text-xl text-center text-[#21243D] dark:text-white">Back-End Development</div>
                      <div class="flex flex-row justify-between">

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>NodeJS</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>CI/CD</div>
                          </div>
                        </div>

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>PHP & SQL</div>
                          </div>
                        </div>

                      </div>
                    </div>
                  </div>
                </div>

                <div class="sm:flex sm:flex-row sm:space-x-9">
                  <!-- Tools & Other stuff -->
                  <div>
                    <div class="flex flex-col">
                      <div class="py-2 montserrat font-bold text-xl text-center text-[#21243D] dark:text-white">Tools & Other stuff</div>
                      <div class="flex flex-row justify-between">

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>Git</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>Figma</div>
                          </div>
                        </div>

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>Photoshop</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>Agility</div>
                          </div>
                        </div>

                      </div>
                    </div>
                  </div>

                  <!-- Languages -->
                  <div>
                    <div class="flex flex-col">
                      <div class="py-2 px-14 montserrat font-bold text-xl text-center text-[#21243D] dark:text-white">Languages</div>
                      <div class="flex flex-row justify-between">

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>French</div>
                          </div>
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>English</div>
                          </div>
                        </div>

                        <div class="flex flex-col space-y-4 text-gris dark:text-gris">
                          <div class="flex flex-row items-center space-x-2">
                            <img src="@/assets/icons/check.svg" alt="îcone validé">
                            <div>Spanish</div>
                          </div>
                        </div>

                      </div>
                    </div>
                  </div>
                </div>

            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VNavbar",
  data() {
    return {
      openTab: 1
    }
  },
  methods: {
    toggleTabs: function(tabNumber){
      this.openTab = tabNumber
      console.log("Current directory:", __dirname);
    }
  }
}
</script>