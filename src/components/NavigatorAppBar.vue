<template>
  <v-app-bar>
    <router-link to="/" class="text-black space-from-left">
      <v-app-bar-nav-icon>
        <v-img :src="require('../assets/l@2x.png')" height="40" width="40"/>
      </v-app-bar-nav-icon>
    </router-link>

    <v-spacer></v-spacer>

    <router-link to="" class="text-black text-decoration-none nav-bar" @click.stop="drawer = !drawer">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </router-link>
  </v-app-bar>

  <v-navigation-drawer
      v-model="drawer"
      bottom
      width="200"
  >
    <v-list-item class="justify-center overflow-hidden">
      <router-link to="/" class="text-black text-decoration-none">
        <v-btn>
          <v-app-bar-title>
            <span class="ma-2 text-size font-weight-bold">Steaks</span>
          </v-app-bar-title>
        </v-btn>
      </router-link>
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
      <router-link to="/" class="text-black text-decoration-none">
        <v-btn>
          <v-app-bar-title>
            <span class="ma-2 text-size font-weight-bold">Burgers</span>
          </v-app-bar-title>
        </v-btn>
      </router-link>
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
      <router-link to="/" class="text-black text-decoration-none">
        <v-btn>
          <v-app-bar-title>
            <span class="ma-2 text-size font-weight-bold">French fires</span>
          </v-app-bar-title>
        </v-btn>
      </router-link>
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
      <router-link to="/" class="text-black text-decoration-none">
        <v-btn>
          <v-app-bar-title>
            <span class="ma-2 text-size font-weight-bold">Drinks</span>
          </v-app-bar-title>
        </v-btn>
      </router-link>
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
      <router-link to="/" class="text-black text-decoration-none">
        <v-btn>
          <v-app-bar-title>
            <span class="ma-2 text-size font-weight-bold">Gdzie dowozimy?</span>
          </v-app-bar-title>
        </v-btn>
      </router-link>
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
      <router-link to="/" class="text-black text-decoration-none">
        <v-btn>
          <v-app-bar-title>
            <span class="ma-2 text-size font-weight-bold">Kontakt</span>
          </v-app-bar-title>
        </v-btn>
      </router-link>
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
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
    </v-list-item>

    <v-list-item class="justify-center overflow-hidden">
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
    </v-list-item>

    <v-list-item class="justify-center space-left overflow-hidden">
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
    </v-list-item>
  </v-navigation-drawer>
</template>

<script>
export default {
  name: "NavigatorAppBar",
  data() {
    return {
      drawer: false,
    }
  }
}
</script>

<style lang="scss">
.space-left {
  margin-left: 35px;
}
</style>
