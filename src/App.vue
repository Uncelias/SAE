<template>
  <!--HEADER AVEC L'ICONE MENU RESPONSIVE!-->

  <div class="bg-black">
    <imghead class="w-full" />
    <div class="flex flex-grow-0 flex-shrink-0 bg-black">
      <div class="font-inter flex-grow space-x-3">
        <nav class="hidden lg:flex lg:gap-8">
          <ul class="flex-grow flex space-x-7 text-base font-medium mt-3 ml-11">
            <li>
              <router-link to="/">Rent</router-link>
            </li>
            <li>
              <router-link to="/">Buy</router-link>
            </li>
            <li>
              <router-link to="/">Sell </router-link>
            </li>
            <li>
              <router-link to="/">Manage Property</router-link>
            </li>
            <li>
              <router-link to="/">Resources</router-link>
            </li>
          </ul>
        </nav>

        <div class="mt-4 ml-10 absolute top-0 right-0 mr-4">
          <menuicon class="lg:hidden" />
        </div>
        <titrepage class="flex justify-center" />
      </div>
      <div class="hidden">
        <p
          class="
            flex
            rounded-lg
            text-indigo-700
            font-semibold
            p-2
            border-indigo-300 border-4
          "
        >
          Login
        </p>
        <p class="flex rounded-lg bg-indigo-600 text-white font-semibold p-3">
          Sign up
        </p>
      </div>
    </div>
    <div class="flex flex-col lg:flex-row justify-between lg:items-center">
      <!--TAG LINE!-->

      <p class="flex text-white font-space-age text-2xl -mt-14 ml-8">
        Join The Move
      </p>
      <p class="flex text-white font-inter ml-8 mr-8">
        Take part to the first edition of UTOPIA the new electro fest coming to
        london this summer !
      </p>

      <p
        class="
          flex flex-row-reverse
          text-white
          font-space-age
          text-2xl
          mt-14
          mr-8
        "
      >
        Be Ready
      </p>
      <p class="flex flex-row-reverse font-inter text-white ml-8 mr-8">
        From the 20th of august to the 22th come
      </p>
      <p class="flex flex-row-reverse font-inter text-white ml-8 mr-8">
        assist the biggest electro fest in Europe !
      </p>

      <p class="flex text-white text-2xl font-space-age mt-14 ml-8">
        Who's in?
      </p>
      <p class="flex text-white ml-8 font-inter mr-8">
        We've brought back the best DJs to make you electrize!
      </p>

      <!--CAROUSEL-->

      <section
        class="relative w-full flex gap-6 snap-x overflow-x-auto pb-14 mt-7"
      >
        <div class="snap-center shrink-0">
          <div class="shrink-0 w-4 sm:w-48"></div>
        </div>
        <div class="snap-center shrink-0 first:pl-8 last:pr-8">
          <img
            class="shrink-0 w-80 h-40 rounded-lg shadow-xl bg-black"
            src="./assets/david.png"
          />
        </div>
        <div class="snap-center shrink-0 first:pl-8 last:pr-8">
          <img
            class="shrink-0 w-80 h-40 rounded-lg shadow-xl bg-black"
            src="./assets/deadmau.png"
          />
        </div>
        <div class="snap-center shrink-0 first:pl-8 last:pr-8">
          <img
            class="shrink-0 w-80 h-40 rounded-lg shadow-xl bg-black"
            src="./assets/martin.png"
          />
        </div>
        <div class="snap-center shrink-0 first:pl-8 last:pr-8">
          <img
            class="shrink-0 w-80 h-40 rounded-lg shadow-xl bg-black"
            src="./assets/djsnake.png"
          />
        </div>

        <div class="snap-center shrink-0">
          <div class="shrink-0 w-4 sm:w-48"></div>
        </div>
      </section>

      <!--CAROUSEL-->

      <div class="justify-content align-middle text-center">
        <p class="block text-white text-2xl font-space-age mt-4">
          Take your ticket
        </p>
      </div>

      <!--SEARCH BAR ET SEARCH LOCATION RESPONSIVE!-->
      <card />
      <card2 />
      <card3 />

      <div class="pl-8 pt-4 pr-8 lg:flex-auto lg:max-w-sm">
        <searchBar />
      </div>
    </div>

    <div class="pl-8 pt-6 pr-8 pb-8 lg:hidden">
      <searchlocation />
    </div>

    <div
      class="
        grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(500px,1fr))]
      "
    ></div>

    <!--ICONES ET FLECHES PERMETTANT DE CHANGER DE PAGES + RESPONSIVE!-->
  </div>

  <!--FOOTER MOBILE FIRST NON RESPONSIVE!-->

  <hr class="bg-white" />
  <footer class="flex flex-col text-center bg-black pt-2">
    <p class="text-white font-space-age text-xl ml-8 mr-8">
      Subscribe to the newsletter
    </p>
    <btnfoot
      class="text-white font-space-age text-2xl ml-8 mr-8 mt-4 mb-4"
      btn="SUBSCRIBE HERE"
    ></btnfoot>
    <p class="text-white font-space-age text-2xl">FOLLOW US !</p>
    <div class="flex justify-center">
      <facebook></facebook>
      <instagram></instagram>
      <twitter></twitter>
    </div>
    <btnfoot
      class="text-white font-space-age text-2xl ml-8 mr-8 mt-4 mb-4"
      btn="CONTACT"
    ></btnfoot>
  </footer>
</template>
<script >
import bouton from "./components/bouton.vue";
import card from "./components/card.vue";
import card2 from "./components/card2.vue";
import card3 from "./components/card3.vue";
import card4 from "./components/card4.vue";
import footer1 from "./components/footer.vue";
import searchBar from "./components/searchbar.vue";
import header1 from "./components/header1.vue";
import menu from "./components/menu.vue";
import searchlocation from "./components/searchlocation.vue";
import pagebar from "./components/pagebar.vue";
import arrow1 from "./components/icones/arrowleft.vue";
import arrow2 from "./components/icones/arrowright.vue";
import threedot from "./components/icones/threedot.vue";
import menuicon from "./components/icones/menuicon.vue";
import titrepage from "./components/titrepage.vue";
import imghead from "./components/imghead.vue";
import searchicon from "./components/icones/searchicon.vue";
import btnfoot from "./components/btn_foot.vue";
import facebook from "./components/icones/facebook.vue";
import instagram from "./components/icones/instagram.vue";
import twitter from "./components/icones/twitter.vue";

export default {
  name: "App",
  components: {
    bouton,
    card,
    card2,
    card3,
    card4,
    footer1,
    searchBar,
    header1,
    titrepage,
    menu,
    imghead,
    searchlocation,
    pagebar,
    arrow1,
    arrow2,
    threedot,
    menuicon,
    btnfoot,
    facebook,
    instagram,
    twitter,
  },
};
</script>