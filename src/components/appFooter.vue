<template>
  <v-card>
    <v-footer dark class="font-weight-medium" color="#707070">
      <v-col class="text-center" cols="12">
        <!--<v-btn
          text
          class="text-uppercase"
          href="https://damonb.dev"
          target="_blank"
          >--><strong>Infinite Auto Tech, LLC&copy;</strong
        ><!--</v-btn
        >-->&nbsp;{{ new Date().getFullYear() }}
      </v-col>
    </v-footer>
  </v-card>
</template>
<script>
export default {
  name: "AppFooter"
};
</script>

<style scoped>
.link,
a {
  color: white;
}
</style>
