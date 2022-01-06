<template>
  <article>
    <section class="pl-10">
      <img
        class="object-cover h-full w-full"
        style="height: 300px"
        :src="image"
        alt="Sport"
      />

      <div class="flex justify-between py-3 text-xs">
        <p class="text-black bg-white p-2 rounded-full px-4 text-center">
          {{ category }}
        </p>
        <p
          v-if="promote"
          class="text-black bg-white p-2 mr-20 rounded-full px-4 text-center"
        >
          Mise en avant
        </p>
        <p class="text-gray-400">
          {{ publication }}
        </p>
      </div>

      <div>
        <p class="text-xl font-medium">{{ paragraph }}</p>
        <p>{{ description }}</p>
      </div>
    </section>
  </article>
</template>

<script>
export default {
  name: 'VBlogCard',

  props: {
    promote: {
      type: Boolean,
      default: false,
    },

    image: {
      type: String,
      required: true,
    },

    category: {
      type: String,
      required: true,
    },

    publication: {
      type: String,
      required: true,
    },

    paragraph: {
      type: String,
      required: true,
    },

    description: {
      type: String,
      required: true,
    },
  },
}
</script>
