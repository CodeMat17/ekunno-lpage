<template>
<div class="flex-1">
  <div
    id="home"
    class="bg-cover bg-center w-full h-screen"
    :style="{
      'background-image': `url(${require('@/assets/images/bg.webp')})`,
    }"
  >
    <div class="w-full h-screen flex justify-center items-center">
    <div class=" p-8">
      <figure class="sm:flex sm:border-4 sm:border-gray-500 sm:shadow-xl sm:rounded-xl sm:overflow-hidden">
        <img
          class="w-32 h-36 sm:w-48 sm:h-auto rounded-full  sm:rounded-l-lg mx-auto object-cover"
          src="@/assets/images/ekunno.webp"
          alt="profile-photo"
          
        />
        <div class="pt-6 sm:p-8 text-center text-gray-900 sm:max-w-xl sm:text-left space-y-4">
          <figcaption class="font-bold">
            <div class=" text-2xl sm:text-4xl">Mike Ekunno</div>
          </figcaption>
          <blockquote>
            <p class="text-lg font-semibold sm:text-xl">
            Much published, award-winning, creative thinker, writer. Flawed follower of Jesus. Lover of beauty.
            </p>
          </blockquote>
            <div class="flex justify-center items-center sm:justify-start sm:items-start">
                <a href="mailto:chudiekunno@yahoo.com" aria-label="Email" rel="noreferrer">
                  <div
                    class="w-12 h-12 mt-4 mr-6 flex justify-center items-center rounded-full border-4 hover:border-gray-900 text-gray-900 bg-gray-400 animate-bounce"
                  >
                    <img src="@/assets/svg/email.svg" alt="email-svg" class="w-8 h-8" />
                  </div>
                </a>
                <a href="https://facebook.com/mike.ekunno" aria-label="Twitter" rel="noreferrer" target="_blank">
                  <div
                    class="w-12 h-12 mt-4 mr-6 flex justify-center items-center rounded-full border-4 hover:border-gray-900 text-gray-900 bg-gray-400 animate-bounce"
                  >
                    <img src="@/assets/svg/facebook.svg" alt="facebook-svg" class="w-8 h-8" />
                  </div>
                </a>
                <a
                  href="https://www.linkedin.com/in/mike-ekunno-98080a44/" rel="noreferrer" aria-label="LinkedIn"
                  target="_blank"
                >
                  <div
                    class="w-12 h-12 mt-4 flex justify-center items-center rounded-full border-4 hover:border-gray-900 text-gray-900 bg-gray-400 animate-bounce"
                  >
                    <img
                      src="@/assets/svg/linkedin.svg" alt="linkedIn-svg"
                      class="w-8 h-8 fill-current"
                    />
                  </div>
                </a>
              </div>
        </div>
      </figure>
      </div>
    </div>
  </div>

  <!-- ###############About Me##################### -->
  <div id="profile">
    <profile />
  </div>
    <!-- ###############Projects##################### -->
  <div id="projects">
    <projects />
  </div>
    <!-- ###############Contact##################### -->
  <div id="contact">
    <contact />
  </div>
    <!-- ###############Footer##################### -->
  <div>
    <futta />
  </div>
  </div>
</template>

<script>
export default {
    name: "Home",
  head() {
    return {
      title: "Mike-Ekunno",
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        {
          hid: "description",
          name: "description",
          content: "Mike Ekunno Landing Page",
        },
      ],
    };
  },
}
</script>
