<template>
  <div class="bg-gray-400 px-4 py-12">
    <div
      class="uppercase text-gray-900 text-3xl text-center font-bold tracking-wider"
    >
      Recent Projects
    </div>
    <div class="flex mx-auto text-center bg-gray-900 h-1 w-40"></div>
    <div
      class="mt-12 sm:grid sm:grid-cols-2 lg: grid lg:grid-cols-3 xl:grid xl:grid-cols-4 gap-10"
    >
      <div v-for="project in projects" :key="project">
        <div
          class="rounded-xl overflow-hidden mb-8 shadow-xl mx-4 relative bottom-0"
        >
          <img
            class="w-full h-48  object-cover"
            :src="project.image"
            alt="project-img"
          />
          <div class="px-4 pb-1 bg-gray-100">
            <h4
              class="text-teal-900 text-xl sm:text-2xl font-bold tracking-widest"
            >
              {{ project.title }}
            </h4>
            <p
              class="py-1 leading-tight text-gray-600 sm:text-lg font-semibold tracking-wide"
            >
              {{ project.description }}
            </p>
          </div>
          <div class="absolute top-0 ml-4 text-teal-800 text-sm">
            <span
              v-show="project.new"
              class="uppercase mt-4 text-sm bg-teal-200 inline-block py-1 px-2 rounded-full text-teal-800"
            >
              new
            </span>
            <div class="mt-4 bg-teal-200 py-1 px-2 rounded-lg font-bold text-xs">
              <p class="tracking-wider">&bull; Author - {{ project.author }}</p>
              <p class="tracking-wider">
                &bull; Published on - {{ project.published }}
              </p>
            </div>
          </div>
          <div class=""></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          new: true,
          author: "Mike Ekunno",
          published: "March, 2009",
          title: "Lorem ipsum",
          image: require("assets/images/books.webp"),
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto quam perspiciatis fugit?",
        },
        {
          new: false,
          author: "Mike Ekunno",
          published: "Dec, 2011",
          title: "Lorem ipsum.",
          image: require("assets/images/books.webp"),
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto quam perspiciatis fugit?",
        },
        {
          new: false,
          author: "Mike Ekunno",
          published: "Oct, 2018",
          title: "Lorem ipsum.",
          image: require("assets/images/books.webp"),
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto quam perspiciatis fugit?",
        },
        {
          new: false,
          author: "Mike Ekunno",
          published: "Nov, 2019",
          title: "Lorem ipsum.",
          image: require("assets/images/books.webp"),
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto quam perspiciatis fugit?",
        },
      ],
    };
  },
};
</script>
