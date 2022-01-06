<template>
  <article>
    <section class="pl-10">
      <img
        class="object-cover h-full w-full"
        style="height: 300px"
        :src="require(`@/assets/images/sport.jpeg`)"
        alt="Sport"
      />

      <div class="flex justify-between py-3 text-xs">
        <p class="text-black bg-white p-2 rounded-full w-14 text-center">
          Sport
        </p>
        <p class="text-gray-400">
          Publiée le 6 janvier 2022 par Jeremy Tellier
        </p>
      </div>

      <div>
        <p class="text-lg font-medium">Je veux être fort !</p>
        <p>Article sur mon point de vue concernant le gain de force.</p>
      </div>
    </section>
  </article>
</template>

<script>
export default {
  name: 'VBlogCard',
}
</script>

<style scoped></style>
