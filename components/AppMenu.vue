<template>
    <nav>
        <ul>
            <li><nuxt-link exact to="/"><AppLogo/></nuxt-link></li>
            <li><nuxt-link  to="/restaurants">Restaurants</nuxt-link></li>
        </ul>
        <AppCartNum/>
        <nuxt-link to="/cart">Cart</nuxt-link>
    </nav>
</template>

<script>
import AppCartNum from './AppCartNum.vue'
import AppLogo from './AppLogo.vue'
    export default {
  components: { AppLogo, AppCartNum },
        
    }
</script>

<style lang="scss" scoped>

</style>