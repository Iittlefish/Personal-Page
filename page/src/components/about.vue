<template>
  <v-container>
    <v-img src='../resume.jpg'></v-img>
    <router-link to='/'>
    <v-btn elevation="2">Home</v-btn>
  </router-link>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'about',
});
</script>
