<template>
  <v-row>
    <v-col
        cols="12" sm="6"
    >
      <slider/>
    </v-col>
    <v-col
        cols="12" sm="6"
    >
      <v-img :src="require('../assets/Bitmapv.png')" height="400" cover/>
    </v-col>
  </v-row>

  <banner-with-food/>

  <v-row>
    <v-col
        cols="12" sm="6"
    >
      <v-img :src="require('../assets/dana-devolk-x2cNcfz_xXU-unsplash.png')" height="400" cover
             class="img-left">
        <div class="text-white div-left-photo">
          <div class="text-h4 box-left">
            Zestaw dla 3 osób
          </div>
          <div class="text-in-box-left">
            Razem smakuje lepiej! Zamów<br> zestawy obiadowe dla 3 osób<br> już od <span>39 zł</span>
          </div>
          <v-btn
              color="#920303"
              class="btn text-white"
              width="160"
          >
            Zamów online
          </v-btn>
        </div>
      </v-img>
    </v-col>

    <v-col
        cols="12" sm="6"
    >
      <v-img :src="require('../assets/aplikacja@2x.png')" height="400" cover class="img-right">
        <div class="text-white div-right-photo">
          <div class="text-h4 box-right">
            UberEats
          </div>
          <div class="text-in-box-right">
            Zamawiaj w aplikacji <span>10% taniej.</span><br> Pobierz aplikację UberEats już dziś.
          </div>

          <div class="d-flex icon-shop">
            <v-img :src="require('../assets/Group 4.svg')" height="20" width="20"/>
            <v-img :src="require('../assets/App_Store_(iOS).svg')" height="20" width="20"/>
            <v-img :src="require('../assets/huawei-app-badge-9757fa 2.svg')" height="20" width="20"/>
          </div>
          <v-btn
              color="#920303"
              class="btn text-white"
              width="160"
          >
            Zamów online
          </v-btn>
        </div>
      </v-img>
    </v-col>
  </v-row>
</template>
<script>


import Slider from "@/components/Slider";
import BannerWithFood from "@/components/BannerWithFood";

export default {
  name: 'HomeView',
  components: {
    BannerWithFood,
    Slider

  }
}
</script>
<style lang="scss">
.img-right {
  border-radius: 10px;

  .div-right-photo {
    margin-left: 6vw;

    .icon-shop {
      width: 100px;
      margin-top: 2vh;
      margin-left: -0.3vw;
    }

    .btn {
      margin-top: 2vh;
    }

    .box-right {
      padding-top: 7vh;
    }

    .text-in-box-right {
      margin-top: 2vh;
      width: 260px;

      span {
        background-color: #920303;
      }
    }
  }
}

.img-left {
  margin-left: 2vw;
  border-radius: 10px;

  .div-left-photo {
    margin-left: 6vw;

    .box-left {
      margin-top: 7vh;
    }

    .text-in-box-left {
      margin-top: 2vh;

      span {
        background-color: black;
        color: white;
      }
    }

    .btn {
      margin-top: 4vh;
    }
  }
}

</style>
