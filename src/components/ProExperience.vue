<template>

    <div class="heebo">
        <h2 class="category circular-std-book text-2xl">Professional experience</h2>

        <div class="text-sm max-w-md">
            <div class="py-4 flex flex-col">
                <div class="text-gray-500">Sept 2021 - Present</div>
                <div class="py-2 flex flex-row">
                    <div>Web Development Apprenticeship</div>
                    <div></div>
                </div>
                <div class="flex flex-row items-center">
                    <div><img class="h-7 w-auto" src="@/assets/imgs/mdf.png" alt="Marketing Digital Facile Logo"></div>
                    <div class="px-2 circular-std-book company">Marketing Digital Facile</div>
                    <div class="sf-pro-display-regular">Freelance Webmaster</div>
                </div>
                <div class="py-2">
                    <div>I have done many tasks at MDF, but my main job was to develop a WordPress Extension</div>
                    <ul class="mt-1 w-fit z-50">
                        <li>
                            <a class="transition-all duration-150 ease-in sf-pro-display-regular text-blue-500 hover:text-blue-600" href="https://www.marketingdigitalfacile.com">www.marketingdigitalfacile.com</a>
                        </li>
                        <li>
                            <a class="transition-all duration-150 ease-in sf-pro-display-regular text-blue-500 hover:text-blue-600" href="https://www.la-caverne-dlp.com">www.la-caverne-dlp.com</a>
                        </li>
                    </ul>
                </div>
            </div>


            <div class="py-4 flex flex-col">
                <div class="text-gray-500">Oct 2020</div>
                <div class="py-2 flex flex-row">
                    <div>Web Development Internship</div>
                    <div></div>
                </div>
                <div class="flex flex-row items-center">
                    <div><img class="h-7 w-auto" src="@/assets/imgs/fireservice.svg" alt="Fireservice Logo"></div>
                    <div class="px-2 circular-std-book company">Fireservice</div>
                    <div class="sf-pro-display-regular">Security guards & Formations</div>
                </div>
                <div class="py-2">
                    <div>During my internship, I was able to create the company's website with a custom WordPress theme and worked on the SEO</div>
                    <ul class="mt-1 w-fit z-50">
                        <li>
                            <a class="transition-all duration-150 ease-in sf-pro-display-regular text-blue-500 hover:text-blue-600" href="https://www.fireservice.fr">www.fireservice.fr</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </div>

</template>

<script>
export default {
  name: 'ProExperience'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.company{
  text-decoration: underline;
  text-underline-offset: 3px;
}
</style>
