<template>
  <v-app>
    <AppNavigation></AppNavigation>
    <Home></Home>
    <AppFooter></AppFooter>
  </v-app>
</template>

<script>
import AppNavigation from "@/components/appNavigation";
import AppFooter from "@/components/appFooter";
import Home from "@/views/Home";

export default {
  name: "App",
  components: {
    AppNavigation,
    Home,
    AppFooter
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
