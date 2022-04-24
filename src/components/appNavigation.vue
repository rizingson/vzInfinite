<template>
  <span>
    <v-navigation-drawer
      app
      v-model="drawer"
      color="#707070"
      dark
      disable-resize-watcher
    >
      <v-list>
        <!-- create list of items, and link them to appropriate view-->

        <!--<router-link to="/Services">
          <v-list-tile class="link" @click="$vuetify.goTo('#more')">
            <v-list-tile-content>
              Services
            </v-list-tile-content>
          </v-list-tile>
        </router-link>-->

        <v-divider></v-divider>

        <router-link to="/location">
          <v-list-tile class="link" @click="$vuetify.goTo('#more')">
            <v-list-tile-content>
              Location
            </v-list-tile-content>
          </v-list-tile>
        </router-link>

        <v-divider></v-divider>

        <!-- <router-link to="/contact">
          <v-list-tile class="link" @click="$vuetify.goTo('#more')">
            <v-list-tile-content>
              Contact
            </v-list-tile-content>
          </v-list-tile>
        </router-link>-->

        <v-divider></v-divider>
      </v-list>
    </v-navigation-drawer>

    <!--navigation bar for regular sized (med and up) displays-->
    <v-app-bar app color="#707070" dark>
      <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer">
      </v-app-bar-nav-icon>

      <!-- make toolbar title a link to return to home page-->
      <router-link to="/">
        <v-img
          class="mx-2"
          :src="require('@/assets/logo.png')"
          max-height="100"
          max-width="100"
          contain
        ></v-img>
      </router-link>

      <!--<v-btn
        depressed
        color="#707070"
        class="link hidden-sm-and-down"
        to="/services"
        @click="$vuetify.goTo('#more')"
        >Services</v-btn
      >
      <v-btn
        depressed
        color="#707070"
        class="link hidden-sm-and-down"
        to="/location"
        @click="$vuetify.goTo('#more')"
        >Location</v-btn
      >-->
      <v-spacer></v-spacer>

      <a class="link hidden-sm-and-down pa-2" href="tel:4089440408"
        >(408) 944-0408</a
      >

      <v-btn
        icon
        href="https://www.yelp.com/biz/infinite-auto-repair-tech-san-jose"
        target="_blank"
      >
        <v-img src="../assets/yelp.png" contain></v-img>
      </v-btn>

      <v-btn
        icon
        href="https://www.facebook.com/infiniteautotech/"
        target="_blank"
      >
        <v-icon class="pa-2" x-large>mdi-facebook</v-icon>
      </v-btn>

      <v-btn icon href="mailto: info@infiniteautotech.com">
        <v-icon class="pa-2" x-large>mdi-email</v-icon>
      </v-btn>

      <v-btn icon @click="$vuetify.goTo('#more')">
        <v-icon class="pa-2" x-large>mdi-map-marker</v-icon>
      </v-btn>
    </v-app-bar>
  </span>
</template>

<script>
export default {
  name: "AppNavigation",
  data() {
    return {
      drawer: false,
      elements: [
        { title: "Services" },
        { title: "Location" },
        { title: "Contact" }
      ]
    };
  }
};
</script>

<style scoped>
a,
.link {
  color: white;
  text-decoration: none;
}
</style>
