<template>
  <v-container fluid fill-height>
    <v-content class="home-page">
      <v-row>
        <v-col sm="12" md="12" class="mx-auto pt-0">
          <homePage></homePage>
        </v-col>
      </v-row>
      <v-row>
        <v-col id="more">
          <Location></Location>
        </v-col>
      </v-row>
    </v-content>
  </v-container>
</template>

<script>
import homePage from "@/components/homePage";
import Location from "@/components/location";
export default {
  name: "Home",
  components: {
    homePage,
    Location
  }
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#about,
#main {
  background-color: whitesmoke;
}

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
</style>
