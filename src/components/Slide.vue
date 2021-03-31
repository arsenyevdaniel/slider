<template>
    <div>
        <v-card width="900" class="mx-auto" elevation="20">
            <v-list-item>
                <v-list-item-content>
                    <v-list-item-title class="headline mb-1">
                        Карточка Instagram
                    </v-list-item-title>
                    <v-list-item>
                        <div>
                            <v-list-item-title class="headline mb-4">
                            </v-list-item-title>
                            <p>Имя: {{Name}}</p>                          
                            <p>Фамилия: {{Surname}}</p>
                            <p>Возраст: {{Age}}</p>
                            <p>Место рождение: {{Location}}</p>
                            <a href=https://www.instagram.com/arsenyevdaniel/>Instagram-></a>
                        </div>
                    </v-list-item>
                </v-list-item-content>
                <v-list-item-avatar size="400">
                    <v-img
                    src="https://sun9-22.userapi.com/impf/c849020/v849020041/624c1/V861qKSk1GI.jpg?size=2048x1360&quality=96&sign=49c710333982fdb63d16e5fd6aab0006&type=album"
                    >
                    </v-img>
                </v-list-item-avatar>
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item>
            <v-card-actions>
               <div>
              <v-btn
               class="ma-2"
              text
               icon
               color="blue lighten-2"
          >
             <v-icon>mdi-thumb-up</v-icon>
           </v-btn>

                <v-btn
                      class="ma-2"
                      text
                      icon
                      color="red lighten-2"
                     >
                     <v-icon>mdi-thumb-down</v-icon>
                 </v-btn>
             </div>

                  

                    <v-btn

                       
                        @click="Show = !Show">
                     >
                        <v-icon dark>
                         mdi-message-text
                         </v-icon>
                    </v-btn>
            </v-card-actions>
            <div>
                <Carusel v-show="Show"/>
            </div>
        </v-card>
    </div>
</template>

<script>
import Carusel from './Carusel'
export default {
    name: "Card",
    components:{
        Carusel
    },
    data: function(){
        return{
            Name: "Даниэль",
            Surname: "Арсеньев",
            Age: "20",
            Location: "Россия",
            Show: false
        }
    }
}
</script>

<style>
#page{
    margin: 5%;
    padding: 5%;
}
</style>