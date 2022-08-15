<template>
  <router-link to="/" class="text-black space-from-left">
    <v-app-bar-nav-icon>
      <v-img :src="require('../assets/l@2x.png')" height="40" width="40"/>
    </v-app-bar-nav-icon>
  </router-link>

  <v-spacer></v-spacer>

  <router-link to="" class="text-black text-decoration-none nav-bar">
    <v-app-bar-nav-icon></v-app-bar-nav-icon>
  </router-link>
</template>

<script>
export default {
  name: "AppBar",
  data() {
    return {}
  }
}
</script>

<style lang="scss">

</style>
