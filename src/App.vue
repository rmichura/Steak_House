<template>
  <v-app>
    <navigatorBar/>
    <v-main>
      <router-view/>
      <home-view/>
    </v-main>
  </v-app>
</template>

<style>
</style>
<script>
import NavigatorBar from "@/components/NavigatorBar";
import HomeView from "@/views/HomeView";
export default {
  components: {NavigatorBar, HomeView},
}
</script>
