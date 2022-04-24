<template>
  <v-row>
    <v-carousel
      eager
      cycle
      hide-delimiters
      :show-arrows="false"
      height="450"
      dark
      xs12
      class="pb-0 mb-0"
    >
      <v-carousel-item
        v-for="(item, i) in items"
        :key="i"
        :src="item.src"
      ></v-carousel-item>
    </v-carousel>
    <v-text class="font-weight-black mx-auto text-uppercase justify">
      Specializing in repair and service for your Audi, VW, BMW, Porsche, Honda,
      Toyota, and most import model vehicles.
    </v-text>
    <v-col class="darken-5 align ml-auto mr-auto mt-n16" cols="12">
      <v-img
        contain
        class="mx-auto pt-0"
        height="480"
        width="600"
        :src="require('@/assets/logo.png')"
      ></v-img>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "homePage",
  data() {
    return {
      //images
      items: [
        {
          src: require("../assets/shop.jpg")
        },
        {
          src: require("../assets/ste313.jpg")
        },
        {
          src: require("../assets/e30s.jpg")
        },
        {
          src: require("../assets/e30.jpg")
        },
        {
          src: require("../assets/ecu.jpg")
        },
        {
          src: require("../assets/swap.jpg")
        },
        {
          src: require("../assets/pulley.jpg")
        },
        {
          src: require("../assets/mclaren.jpg")
        },
        {
          src: require("../assets/tires.jpg")
        },
        {
          src: require("../assets/m3.jpg")
        },
        {
          src: require("../assets/trans.jpg")
        },
        {
          src: require("../assets/bushing.jpg")
        },
        {
          src: require("../assets/bench.jpg")
        }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.link {
  text-decoration: none;
}
</style>
