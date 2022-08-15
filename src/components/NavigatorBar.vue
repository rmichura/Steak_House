<template>
  <v-app-bar
      height="65"
      elevation="4"
      v-if="windowWidth > 1180"
  >
    <router-link to="/" class="text-black space-from-left">
      <v-app-bar-nav-icon>
        <v-img :src="require('../assets/l@2x.png')" height="40" width="40"/>
      </v-app-bar-nav-icon>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 text-size font-weight-bold">Steaks</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 text-size font-weight-bold">Burgers</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 text-size font-weight-bold">French fires</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 text-size font-weight-bold">Drinks</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 text-size font-weight-bold">Gdzie dowozimy?</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 text-size font-weight-bold">Kontakt</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <v-spacer></v-spacer>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn
          height="57"
          width="97"
      >
        <v-card
            height="57"
            width="97"
            elevation="0"
            class="btn-hover"
        >
          <v-icon class="margin-icon">mdi-account</v-icon>
          <v-app-bar-title>
            <div class="ma-2 text-size font-weight-bold">Moje konto</div>
          </v-app-bar-title>
        </v-card>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn
          height="57"
          width="97"
      >
        <v-card
            height="57"
            width="97"
            elevation="0"
            class="btn-hover"
        >
          <v-icon class="margin-icon">mdi-cart</v-icon>
          <v-app-bar-title>
            <div class="ma-2 text-size font-weight-bold">Koszyk</div>
          </v-app-bar-title>
        </v-card>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none space-from-right">
      <v-btn
          height="57"
          width="97"
      >
        <v-card
            height="57"
            width="97"
            color="#920303"
            class="text-white btn-hover"
            elevation="0"
        >
          <div class="img">
            <v-img :src="require('../assets/zamow_ikona.svg')" height="18" width="18"/>
          </div>
          <v-app-bar-title>
            <div class="font-weight-bold">Zamów</div>
          </v-app-bar-title>
        </v-card>
      </v-btn>
    </router-link>
  </v-app-bar>

    <NavigatorAppBar v-else/>
</template>

<script>

import NavigatorAppBar from "@/components/NavigatorAppBar";
export default {
  name: 'NavigatorBar',
  components: {NavigatorAppBar},
  data() {
    return {
      windowWidth: window.innerWidth,
    };
  },
  mounted() {
    window.onresize = () => {
      this.windowWidth = window.innerWidth
    }
  },
};
</script>
<style lang="scss">

.nav-bar {
  margin-right: 8vw;
}

.text-size {
  font-size: 14px;
}

.margin-icon {
  margin-bottom: -1em;
}

.btn-hover:hover {
  background-color: inherit;
}

.space-from-left {
  margin-left: 8vw;
}

.space-from-right {
  margin-right: 8.5vw;

  div {
    font-size: 14px;
  }

  .img {
    margin-top: 0.5em;
    margin-left: 2.7em;
  }
}

</style>
