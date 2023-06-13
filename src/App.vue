<script>
import { RouterLink, RouterView } from 'vue-router'
import NavDrawer from '@/components/NavDrawer.vue'

export default{
  components: {
    NavDrawer
  }
}

</script>

<template>

<!-- 
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/login">Login</RouterLink>
      </nav> -->
      <NavDrawer />



  <RouterView />

</template>

<style scoped>

</style>
