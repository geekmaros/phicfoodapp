<template>
    <main class="container restaurant">
        <div class="restaurantheading">
          <h1>Restaurants</h1>
          <AppSelect @change="selectedRestaurant = $event"/>
        </div>
      
        <AppRestaurantInfo :datasource="filteredRestaurants"></AppRestaurantInfo>
    </main>
</template>

<script>
import { mapState } from 'vuex';
import AppRestaurantInfo from '~/components/AppRestaurantInfo.vue'
import AppSelect from '~/components/AppSelect.vue'
    export default {
        data(){
            return{
                selectedRestaurant: ''
            }
        },
  components: { AppRestaurantInfo, AppSelect },
  computed:{
      ...mapState(["fooddata"]),
      filteredRestaurants(){
          if(this.selectedRestaurant){
              return this.fooddata.filter(el => {
                  let name = el.name.toLowerCase()
                  return name.includes(this.selectedRestaurant)
              })
          }
        return this.fooddata
      }
  }
        
    }
</script>

<style lang="scss" scoped>

</style>