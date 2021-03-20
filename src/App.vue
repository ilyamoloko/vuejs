<template>
  <v-app>
    <MainMenu/>

    <v-main>
      <carusel :items="items"/>

      <MainFooter :icons="icons"/>
    </v-main>
  </v-app>
</template>

<script>


import MainMenu from "./components/MainMenu";
import Carusel from "./components/Carusel";
import MainFooter from "./components/MainFooter";

export default {
  name: 'App',

  components: {MainFooter, Carusel, MainMenu},

  data() {
    return {
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
      items: [
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          title:'БурундукАнтихриста'
        },

        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          title: 'неба'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          title: 'ОРЕЛ'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          title: 'СПАЙСЫ'
        },
      ],
    }
  },
};
</script>
