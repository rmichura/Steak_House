<template>
  <v-app-bar
      height="81"
  >
    <router-link to="/" class="text-black space-from-left">
      <v-app-bar-nav-icon>
        <v-img :src="require('../assets/l@2x.png')" height="40" width="40"/>
      </v-app-bar-nav-icon>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 font-weight-bold">Steaks</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 font-weight-bold">Burgers</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 font-weight-bold">French fires</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 font-weight-bold">Drinks</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 font-weight-bold">Gdzie dowozimy?</span>
        </v-app-bar-title>
      </v-btn>
    </router-link>

    <router-link to="/" class="text-black text-decoration-none">
      <v-btn>
        <v-app-bar-title>
          <span class="ma-2 font-weight-bold">Kontakt</span>
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
            <div class="ma-2 font-weight-bold">Moje konto</div>
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
            <div class="ma-2 font-weight-bold">Koszyk</div>
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
</template>

<script>

export default {
  name: 'AppBar',

  data() {
    return {}
  },
}
</script>
<style lang="scss">

.ma-2 {
  font-size: 14px;
}

.margin-icon {
  margin-bottom: -1em;
}

.btn-hover:hover {
  background-color: inherit;
}

.space-from-left {
  margin-left: 10em;
}

.space-from-right {
  margin-right: 8.5em;

  div {
    font-size: 14px;
  }

  .img {
    margin-top: 0.5em;
    margin-left: 2.7em;
  }
}

</style>
