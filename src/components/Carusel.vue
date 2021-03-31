<template>
  <v-carousel
      :continuous="false"
      :cycle="cycle"
      :show-arrows="true"
      hide-delimiter-background
      delimiter-icon="mdi-minus"
      height="150"
    >
      <v-carousel-item
        v-for="(Comment, i) in Comments"
        :key="i"
      >
          <Comment :Com="Comment"/>
      </v-carousel-item>
    </v-carousel>
</template>

<script>
import Comment from './Comment.vue'
export default {
    name: 'Carusel',
    components:{
      Comment
    },
    data: function(){
        return{
            model: 0,
          Comments: [
            {
                UserName: 'Сергей', Massage: 'Топ за свои деньги!'
            },
            {
                UserName: 'Кристина', Massage: 'Есть куда рости'
            },
            {
                UserName: 'Иван', Massage: 'Это кто?'
            }
          ]
        }
    }
}
</script>

<style>
</style>