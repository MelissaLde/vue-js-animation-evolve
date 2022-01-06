<template>
  <div id="app" class="container max-w-6xl mx-auto text-white">
    <header class="py-10 pl-10">
      <h1 class="uppercase text-xl pb-2">
        Conseils sur le sport, santé et nutrition aussi simples que évidents à
        mettre en oeuvre
      </h1>
      <h3 class="text-5xl font-bold uppercase">Liste des articles</h3>
    </header>

    <main>
      <article class="grid grid-cols-2 gap-10">
        <section class="pl-10">
          <img
            class="object-cover h-full w-full"
            style="height: 300px"
            src="./assets/images/sport.jpeg"
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
              L'importance de donner à son organisme la quantité d'eau
              suffisante au quotidien, afin d'évitez la rétention d'eau.
            </p>
          </div>
        </section>
      </article>
    </main>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>
