<template>
  <v-app>
    <v-app-bar
      app
      color="orange"
      elevate-on-scroll
      rounded
      dark
    >
      <div class="d-flex align-center">
        <v-icon x-large>mdi-language-php</v-icon>
        <v-btn color="orange" depressed x-small ></v-btn>
        <v-toolbar-title class="mb-1">php is the best language in the world</v-toolbar-title>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/Iittlefish"
        target="_blank"
        text
      >
        <span class="mr-2">My github</span>
        <v-icon large>mdi-github</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'App',

  data: () => ({
    //
  }),
});
</script>
