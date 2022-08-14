<template>
  <v-app>
    <app-bar/>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<style>
</style>
<script>
import AppBar from "@/components/AppBar";
export default {
  components: {AppBar}
}
</script>
