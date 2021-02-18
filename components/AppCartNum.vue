<template>
   <main>
        <div v-if="cartCount" class="smallnum">
        {{cartCount}}
    </div>
    <div v-else class="">
        No Item in Cart
    </div>
   </main>
</template>

<script>
 import { mapGetters } from 'vuex';
 
 export default {
     computed: {
         ...mapGetters([
             'cartCount',
         ])
     },
 };
</script>

<style lang="scss" scoped>

</style>