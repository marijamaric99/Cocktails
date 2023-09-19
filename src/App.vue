<template>
  <v-app id="inspire">
   

    <v-main>
    <router-view/>
    </v-main>

  <v-bottom-navigation style="background-color: rgb(244, 244, 244);">
        <v-btn @click="toFacebook()">
          <v-icon >mdi-facebook</v-icon>
        </v-btn>

        <v-btn @click="toInstagram()">
          <v-icon>mdi-instagram</v-icon>
        </v-btn>

        <v-btn @click="toTwitter()">
          <v-icon>mdi-twitter</v-icon>
        </v-btn>
     </v-bottom-navigation>

      <v-btn
        fab
        dark
        fixed
        bottom
        right
        color="black"
        @click="returnToTop"
      >
        <v-icon>mdi-arrow-up</v-icon>
      </v-btn>

  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
  methods: {
      toFacebook: function(){
        window.open('https://www.facebook.com/Cocktails.Cocktails.Cocktails')
      },
       toInstagram: function(){
        window.open('https://www.instagram.com/cocktails/')
      },
       toTwitter: function(){
        window.open('https://www.instagram.com/cocktails/')
      },
      returnToTop: function(){
        window.scrollTo(0, 0);
      }
    },
};
</script>
