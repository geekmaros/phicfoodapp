<template>
    <nav>
        <ul>
            <li><nuxt-link exact to="/"><AppLogo/></nuxt-link></li>
            <li><nuxt-link  to="/restaurants">Restaurants</nuxt-link></li>
        </ul>
        <AppCartNum v-if="cartCount > 0"/>
        <nuxt-link to="/cart">Cart</nuxt-link>
    </nav>
</template>

<script>
import { mapGetters } from 'vuex';

import AppCartNum from './AppCartNum.vue'
import AppLogo from './AppLogo.vue'
    export default {
  components: { AppLogo, AppCartNum },
  computed: {
      ...mapGetters(['cartCount'])
  }
        
    }
</script>

<style lang="scss" scoped>

</style>