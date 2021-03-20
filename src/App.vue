<template>
  <v-app>
    <MainMenu/>

    <v-main>
      <carusel :items="items"/>
    </v-main>
  </v-app>
</template>

<script>


import MainMenu from "./components/MainMenu";
import Carusel from "./components/Carusel";

export default {
  name: 'App',

  components: {Carusel, MainMenu},

  data() {
    return {
      items: [
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
        },
      ],
    }
  },
};
</script>
