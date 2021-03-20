<template>
  <v-carousel
      cycle
      hide-delimiters
      height="200"
      show-arrows-on-hover
  >
    <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
    >
      <template v-slot:default>
        <v-parallax     height="200"
                        :src="item.src">

          <v-row

              class="fill-height"
              align="center"
              justify="center"
          ><span class="mytitlesliderman">Это слайд</span>
          </v-row>
        </v-parallax>
      </template>






    </v-carousel-item>
  </v-carousel>
</template>
<script>
export default {
  name: 'carusel',
  props: {
    items: {}
  }
}
</script>

<style>
.mytitlesliderman{
  font-size: 72px;
}
</style>