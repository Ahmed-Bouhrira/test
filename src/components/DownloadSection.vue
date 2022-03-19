<template>
  <section id="download">
    <template>
      <v-carousel hide-delimiters>
        <v-carousel-item
          v-for="(item, i) in items"
          :key="i"
          :src="item.src"
        ></v-carousel-item>
      </v-carousel>
    </template>
  </section>
</template>

<style scoped>
#download .container,
#download .row {
  height: 100%;
}
</style>
<script>
export default {
  data() {
    return {
      items: [
        {
          src: require("@/assets/img/carou.png")
        },
        {
          src: require("@/assets/img/carou2.png")
        },
        {
          src: require("@/assets/img/carous3.png")
        },
        {
          src: require("@/assets/img/carou4.png")
        }
      ]
    };
  }
};
</script>
