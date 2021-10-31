<template>
  <about />
</template>

<script lang="ts">
import Vue from 'vue';
import about from '../components/about.vue';

export default Vue.extend({
  name: 'Home',

  components: {
    about,
  },
});
</script>
