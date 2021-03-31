<template>
  <v-app>
    <v-main>
      <Slide/>
    </v-main>
  </v-app>
</template>

<script>

import Slide from './components/Slide.vue';
export default {
  name: 'App',
  components: {

    Slide,
  },
  data: () => ({
    //
  }),
};
</script>