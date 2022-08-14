<template>
  <v-app>
    <app-bar/>
    <v-main>
      <router-view/>
      <home-view/>
    </v-main>
  </v-app>
</template>

<style>
</style>
<script>
import AppBar from "@/components/AppBar";
import HomeView from "@/views/HomeView";
export default {
  components: {HomeView, AppBar}
}
</script>
