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
        reverse-transition="fade-transition"
        transition="fade-transition"

    ></v-carousel-item>
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