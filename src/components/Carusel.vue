<template>
  <v-carousel
      cycle
      hide-delimiters
      height="650"
      show-arrows-on-hover
  >
    <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
    >

        <v-row

            class="fill-height"
            align="center"
            justify="center"
        ><span class="mytitlesliderman">{{item.title}}</span>
        </v-row>




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