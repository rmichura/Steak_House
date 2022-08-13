<template>
  <v-app>
    <v-main>
      <AppBar/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/AppBar.vue'
import AppBar from "@/components/AppBar";

export default {
  name: 'App',

  components: {
    AppBar,
  },

  data: () => ({
    //
  }),
}
</script>
