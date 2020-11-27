<template>
  <div class="px-4 py-12">
    <div
      class="uppercase text-gray-900 text-3xl text-center font-bold tracking-wider"
    >
      Need an Editor?
    </div>
    <div class="flex mx-auto bg-gray-900 h-1 w-40"></div>
    <p class="mt-4 text-center text-gray-600 text-xl font-bold italic">
      ~ I'm your man. Reach me by tapping on any of the buttons below ~
    </p>
    <div class="sm:flex justify-center items-center">
      <div class="mt-16 sm:mr-24">
        <a
          href="mailto:chudiekunno@yahoo.com"
          aria-label="Email"
          rel="noreferrer"
        >
          <div
            class="w-24 h-24 mx-auto flex justify-center items-center rounded-full border-4 border-white shadow-xl animate-bounce"
          >
            <img src="@/assets/svg/email.svg" alt="email-icon" class="relative w-12 h-12" />
          </div>
          <p class="text-center mt-2 font-bold uppercase">email</p>
        </a>
      </div>

      <div class="mt-16 sm:mr-24">
        <a
          href="https://facebook.com/mike.ekunno"
          aria-label="Twitter"
          rel="noreferrer"
          target="_blank"
        >
          <div
            class="w-24 h-24 mx-auto flex justify-center items-center rounded-full border-4 border-white shadow-xl animate-bounce"
          >
            <img src="@/assets/svg/facebook.svg" alt="facebook-icon" class="relative w-12 h-12" />
          </div>
          <p class="text-center mt-2 font-bold uppercase">
            facebook
          </p>
        </a>
      </div>

      <div class="mt-16">
          <a
                  href="https://www.linkedin.com/in/mike-ekunno-98080a44/" rel="noreferrer" aria-label="LinkedIn"
                  target="_blank"
                >
        <div
          class="w-24 h-24 mx-auto flex justify-center items-center rounded-full border-4 border-white shadow-xl animate-bounce"
        >
          <img src="@/assets/svg/linkedin.svg" alt="linkedin-icon" class="relative w-12 h-12" />
        </div>
        <p class="text-center mt-2 font-bold uppercase">linkedIn</p>
          </a>
      </div>
    </div>   
  </div>
</template>

<script>
export default {

};
</script>