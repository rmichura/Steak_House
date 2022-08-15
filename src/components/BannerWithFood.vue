<template>
  <div class="imgs">
    <v-row class="ma-2">
      <v-img :src="require('../assets/Bitmap-4.png')" width="70" height="33"/>
      <v-img :src="require('../assets/e.png')" width="87" height="19" class="ma-2"/>
      <v-img :src="require('../assets/Bitmap.png')" width="79" height="37"/>
      <v-img :src="require('../assets/Bitmap-2.png')" width="107" height="37"/>
      <v-img :src="require('../assets/Bitmap-3.png')" width="86" height="43"/>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "BannerWithFood"
}
</script>

<style lang="scss">
.imgs {
  margin-left: 15vw;
  margin-right: 10vw;
}
</style>
