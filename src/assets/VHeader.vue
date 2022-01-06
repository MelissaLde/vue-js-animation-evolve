<template>
  <header class="py-10 pl-10">
    <h2 class="uppercase text-xl pb-2">
      {{ title }}
    </h2>

    <h3 class="text-5xl font-bold uppercase">{{ subtitle }}</h3>
  </header>
</template>

<script>
export default {
  name: 'VHeader',

  props: {
    title: {
      type: String,
      required: true,
    },

    subtitle: {
      type: String,
      required: true,
    },
  },
}
</script>
