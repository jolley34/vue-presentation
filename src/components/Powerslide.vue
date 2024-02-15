<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Powerslide",
  data() {
    return {
      years: [2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023],
      versions: [
        "0.6 | 0.7",
        "0.8 | 0.9 | 0.10 | 0.11",
        "0.12 | 1.0",
        "2.0 | 2.1",
        "2.2 | 2.3 | 2.4 | 2.5",
        "Nothing new",
        "2.6",
        "3.0",
        "3.1 | 3.2",
        "2.7",
        "3.3 | 3.4",
      ],
    };
  },
});
</script>
<template>
  <div class="grid-container">
    <div
      class="card bg-zinc-700 bg-opacity-20 p-10 px-6 rounded-xl flex justify-between"
    >
      <div class="flex flex-col justify-between">
        <div>
          <h1 class="text-zinc-300 text-6xl">Vad är Vue.js?</h1>
          <p class="text-zinc-400 py-6 text-3xl">
            Vue.js har release 2014 i februari, skapat av Evan You.
          </p>
          <p class="text-zinc-500 text-xl">
            Evan You jobbade för Google där han använde Angular.js, tog de han
            gillade med Angular och gjorde ett förenklat verktyg.
          </p>
        </div>
        <div class="flex flex-col">
          <div class="verion-title text-zinc-500 text-xl hidden">Versions</div>
          <div
            class="timeline-container rounded-lg bg-zinc-600 bg-opacity-20 p-4"
          >
            <div
              class="years font-semibold border-b-2 border-zinc-500 py-2 text-left"
            >
              <h1
                v-for="year in years"
                :key="year"
                class="text-lg text-zinc-400"
              >
                {{ year }}
              </h1>
            </div>
            <div class="versions bg-zinc-800 bg-opacity-50 text-left">
              <h1
                v-for="version in versions"
                :key="version"
                class="text-lg text-zinc-500"
              >
                {{ version }}
              </h1>
            </div>
          </div>
        </div>
      </div>
      <img
        class="rounded-xl drop-shadow-xl"
        src="../assets/evan-you.png"
        alt=""
      />
    </div>
    <div
      class="card bg-zinc-700 bg-opacity-20 p-10 px-6 rounded-xl flex justify-between"
    >
      <div class="flex flex-col justify-between">
        <div>
          <h1 class="text-zinc-300 text-6xl">Varför Vue.js?</h1>
          <p class="text-zinc-400 py-6 text-3xl">Lätt att lära sig</p>
          <p class="text-zinc-500 text-xl">
            Lättförståelig syntax som gör det enkelt att komma igång för
            nybörjare.
          </p>
          <p class="text-zinc-400 py-6 text-3xl">Flexibilitet</p>
          <p class="text-zinc-500 text-xl w-10/12">
            Kan användas som ramverk för bygga en stor ensidig applikation
            (SPA), men också ett enkelt biblotek för att lägga till interaktiva
            saker i en befintlig hemsida.
          </p>
        </div>
      </div>
      <img
        class="rounded-xl drop-shadow-xl"
        src="../assets/whyvue.jpeg"
        alt=""
      />
    </div>
    <div
      class="card bg-zinc-700 bg-opacity-20 p-10 px-6 rounded-xl flex justify-between"
    >
      <div class="flex flex-col justify-between">
        <div>
          <h1 class="text-zinc-300 text-6xl">Syntax</h1>
          <p class="text-zinc-400 py-6 text-3xl">Template</p>
          <p class="text-zinc-500 text-xl">
            Vue.js använder en HTML-baserad template-syntax för att definiera
            användargränssnittet
          </p>
          <p class="text-zinc-400 py-6 text-3xl">Komponenter</p>
          <p class="text-zinc-500 text-xl w-10/12">
            Vue.js använder sig av återanvändbara kompontenter som kan ha sin
            egen logik och stil. Dessa kompontenter defineras i en "script" tag.
          </p>
          <p class="text-zinc-400 py-6 text-3xl">Direktiv</p>
          <p class="text-zinc-500 text-xl w-10/12">
            Inbyggda direktiv som gör att du kan binda data till DOM-attribut ,
            Direktiven används i HTML-koden med hjälp av prefixet v-, en for
            each loop kan t.ex se ut v-for="survey in framework.surveys"
          </p>
        </div>
      </div>
      <img
        class="rounded-xl drop-shadow-xl"
        src="../assets/screenshot-1.png"
        alt=""
      />
    </div>
    <div
      class="card bg-zinc-700 bg-opacity-20 p-10 px-6 rounded-xl flex justify-between"
    >
      <div class="flex flex-col justify-between">
        <div>
          <h1 class="text-zinc-300 text-6xl">Prestanda</h1>
          <p class="text-zinc-400 py-6 text-3xl">Snabbhet</p>
          <p class="text-zinc-500 text-xl pb-4">
            Vue.js är känt för sin snabbhet och prestanda tack vare dess
            virtuella DOM.
          </p>
          <p class="text-zinc-500 text-xl w-10/12">
            Det gör det möjligt att bygga snabba och effektiva webbapplikationer
            även med stora dataset.
          </p>
        </div>
      </div>
      <img
        class="rounded-xl drop-shadow-xl"
        src="../assets/speed.jpeg"
        alt=""
      />
    </div>
    <div
      class="card bg-zinc-700 bg-opacity-20 p-10 px-6 rounded-xl flex justify-between"
    >
      <div class="flex flex-col justify-between">
        <div>
          <h1 class="text-zinc-300 text-6xl">Framtid</h1>
          <p class="text-zinc-400 py-6 text-3xl">Community</p>
          <p class="text-zinc-500 text-xl pb-4">
            Många utvecklare världen över använder och tycker vue.js är bra,
            vilket gör att feedback och nya funktioner hela tiden vill
            förbättras.
          </p>
          <p class="text-zinc-400 py-6 text-3xl">Underhåll</p>
          <p class="text-zinc-500 text-xl pb-4">
            Vue består av en grupp utvecklare som ser till att vue hela tiden
            bli bättre och utvecklas.
          </p>
        </div>
      </div>
      <img
        class="rounded-xl drop-shadow-xl"
        src="../assets/repair.png"
        alt=""
      />
    </div>
    <div
      class="card bg-zinc-700 bg-opacity-20 p-10 px-6 rounded-xl flex justify-between"
    >
      <div class="flex flex-col justify-between">
        <div>
          <h1 class="text-zinc-300 text-6xl">State of Javascript</h1>
          <p class="text-zinc-400 py-6 text-3xl">Pages Upload Inprogress...</p>
          <p class="text-zinc-500 text-xl pb-4">Built with Vue.js OFC</p>
        </div>
      </div>
      <img
        class="rounded-xl drop-shadow-xl"
        src="../assets/state-of-javascript.png"
        alt=""
      />
    </div>
  </div>
</template>

<style scoped>
.grid-container {
  display: grid;
  grid-auto-flow: column;
  grid-auto-columns: 100%;
  overflow-x: scroll;
  scroll-snap-type: x mandatory;
  scroll-padding: 1rem;
  grid-column-gap: 2.5rem;
}

.grid-container > * {
  scroll-snap-align: start;
}

.card {
  overflow-x: scroll;
  font-size: 2rem;
}

.years {
  display: grid;
  align-items: center;
  grid-template-columns: repeat(11, 95px);
}

.versions {
  display: grid;
  grid-template-columns: repeat(11, 95px);
}

@media screen and (max-width: 1100px) {
  .card img {
    display: none;
  }

  .years {
    display: none;
  }

  .versions {
    grid-template-columns: repeat(2, 1fr);
  }

  .verion-title {
    display: block;
  }
}
</style>
