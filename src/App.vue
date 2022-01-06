<template>
  <main id="app" class="container max-w-6xl mx-auto text-white">
    <v-header
      title="Conseils sur le sport, santé et nutrition aussi simples que évidents à
      mettre en oeuvre"
      subtitle="Liste des articles"
    />

    <article class="grid grid-cols-2 gap-10">
      <v-blog-card />

      <section>
        <img
          class="object-cover h-full w-full"
          style="height: 300px"
          src="./assets/images/surf.jpeg"
          alt="Sport"
        />

        <div class="container max-w-xl flex justify-between py-3 text-xs">
          <p class="text-black bg-white p-2 rounded-full w-18 text-center">
            Welness
          </p>
          <p class="text-gray-400">
            Publiée le 6 janvier 2022 par Jeremy Tellier
          </p>
        </div>

        <div>
          <p class="text-lg font-medium">
            Rétention d'eau ? La solution, boire de l'eau !
          </p>
          <p>
            L'importance de donner à son organisme la quantité d'eau suffisante
            au quotidien, afin d'évitez la rétention d'eau.
          </p>
        </div>
      </section>
    </article>

    <v-header title="Hello" subtitle="Lorem ipsum" />

    <article class="grid grid-cols-2 gap-10">
      <v-blog-card />

      <v-blog-card />

      <v-blog-card />

      <v-blog-card />

      <v-blog-card />

      <v-blog-card />

      <v-blog-card />

      <v-blog-card />
    </article>
  </main>
</template>

<script>
import VHeader from '@/assets/VHeader'
import VBlogCard from '@/assets/VBlogCard'

export default {
  name: 'App',

  components: { VHeader, VBlogCard },
}
</script>
