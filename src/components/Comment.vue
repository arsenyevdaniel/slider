<template>
  <v-card width="900" class="mx-auto" elevation="10" >
      <v-list-item>
          <vue-list-title>
              {{Com.UserName}} : {{Com.Massage}} 
          </vue-list-title>
          <v-spacer></v-spacer>
      </v-list-item>
  </v-card>
</template>

<script>
export default {
    name: 'Comment',
    props: ['Com'],
}
</script>
<style>
</style>