<template>
  <main id="app" class="container max-w-6xl mx-auto text-white">
    <v-header
      title="Conseils sur le sport, santé et nutrition aussi simples que évidents à
      mettre en oeuvre"
      subtitle="Liste des articles"
    />

    <article class="grid grid-cols-2 gap-10">
      <v-blog-card
        :promote="promotedBlogPost.promote"
        :image="promotedBlogPost.image"
        :category="promotedBlogPost.category"
        :publication="promotedBlogPost.publication"
        :paragraph="promotedBlogPost.paragraph"
        :description="promotedBlogPost.description"
      />
    </article>

    <v-header title="Hello" subtitle="Lorem ipsum" />

    <article class="grid grid-cols-2 gap-10">
      <v-blog-card
        v-for="blog in promotedBlogPostFalse"
        :key="blog.paragraph"
        :image="blog.image"
        :category="blog.category"
        :publication="blog.publication"
        :paragraph="blog.paragraph"
        :description="blog.description"
      />
    </article>
  </main>
</template>

<script>
import VHeader from '@/components/VHeader'
import VBlogCard from '@/components/VBlogCard'

export default {
  name: 'App',

  components: { VHeader, VBlogCard },

  data: () => ({
    blogs: [
      {
        promote: true,
        image: require(`@/assets/images/sport.jpeg`),
        category: 'Sport',
        publication: 'Publiée le 6 janvier 2022 par Jeremy Tellier',
        paragraph: 'Je veux être fort !',
        description:
          'Article sur mon point de vue concernant le gain de force.',
      },
      {
        promote: false,
        image: require(`@/assets/images/surf.jpeg`),
        category: 'Welness',
        publication: 'Publiée le 6 janvier 2022 par Jeremy Tellier',
        paragraph: "Rétention d'eau ? La solution, boire de l'eau !",
        description:
          "L'importance de donner à son organisme la quantité d'eau suffisante\n" +
          "            au quotidien, afin d'évitez la rétention d'eau.",
      },
      {
        promote: false,
        image: require(`@/assets/images/sport.jpeg`),
        category: 'Sport',
        publication: 'Publiée le 6 janvier 2022 par Jeremy Tellier',
        paragraph: 'Je veux être fort !',
        description:
          'Article sur mon point de vue concernant le gain de force.',
      },
      {
        promote: false,
        image: require(`@/assets/images/surf.jpeg`),
        category: 'Welness',
        publication: 'Publiée le 6 janvier 2022 par Jeremy Tellier',
        paragraph: "Rétention d'eau ? La solution, boire de l'eau !",
        description:
          "L'importance de donner à son organisme la quantité d'eau suffisante\n" +
          "            au quotidien, afin d'évitez la rétention d'eau.",
      },
    ],
  }),

  computed: {
    promotedBlogPost() {
      return this.blogs.find((blog) => blog.promote === true)
    },

    promotedBlogPostFalse() {
      return this.blogs.filter((blog) => blog.promote === false)
    },
  },
}
</script>
