<template>
  <v-row justify="center">
    <v-col
      class="d-flex flex-column flex-grow-0 flex-shrink-0 mt-auto ml-4 pl-0"
    >
      <v-card
        color="#707070"
        max-width="450"
        dark
        class="d-flex flex-column flex-grow-0 flex-shrink-0 justify-start mt-auto pl-0"
      >
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3170.2268469111145!2d-121.91765068448792!3d37.38446724229141!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x808fcbe48283f7ab%3A0x21c14cd4a03869fd!2sInfinite%20Auto%20Tech%2C%20LLC!5e0!3m2!1sen!2sus!4v1614578604885!5m2!1sen!2sus"
          width="450"
          height="300"
          style="border:0"
          frameborder="0"
          allowfullscreen
        ></iframe>
        <v-card-text class="headline text-xs-center text-uppercase">
          Location and Hours
          <hr />
        </v-card-text>
        <v-card-text class="subheading mt-2 text-xs-center">
          Located @ Club Auto Sport in N. San Jose.<br />
          527 Charcot Ave STE 313. <br />
          San Jose, CA 95131<br />
          <br />
          <strong><v-text class="mx-auto justify"> Contact: </v-text></strong
          ><br />
          <v-text class="mx-auto text-uppercase justify">
            info@infiniteautotech.com
          </v-text>
          <br />
          <a class="link" href="tel:4089440408">(408) 944-0408</a>
          <br />
          <br />
          <strong>Business Hours:</strong><br />
          Monday-Friday: 8am to 5pm<br />
          Weekends By Appointment
        </v-card-text>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "location"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.link,
a {
  color: white;
  text-decoration: none;
}
</style>
