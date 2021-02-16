<template>
    <main class="container restaurant">
        <div class="restaurantheading">
          <h1>Restaurants</h1>
          <AppSelect @change="selectedRestaurantInfo = $event"/>
          <pre>{{$data}}</pre>
        </div>
      
        <AppRestaurantInfo></AppRestaurantInfo>
    </main>
</template>

<script>
import AppRestaurantInfo from '~/components/AppRestaurantInfo.vue'
import AppSelect from '~/components/AppSelect.vue'
    export default {
        data(){
            return{
                selectedRestaurantInfo: ''
            }
        },
  components: { AppRestaurantInfo, AppSelect },
        
    }
</script>

<style lang="scss" scoped>

</style>