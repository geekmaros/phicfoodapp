<template>
   <main>
        <div v-if="cartLength" class="smallnum">
        {{cartLength}}
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
             'cartLength',
         ])
     },
 };
</script>

<style lang="scss" scoped>

</style>