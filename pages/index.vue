<template>
  <main class="container">
   <AppHeader></AppHeader>
   <AppRestaurantInfo></AppRestaurantInfo>
  </main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import AppRestaurantInfo from '~/components/AppRestaurantInfo.vue';

export default {
  components: {
    AppHeader,
    AppRestaurantInfo
  },
}
</script>

<style>

</style>
