<template>
  <v-carousel
      cycle
      height="400"
      hide-delimiter-background
      show-arrows="hover"
      color="grey"
  >
    <v-carousel-item
        v-for="(percent, i) in percents"
        :key="i"
    >
      <v-sheet
          height="100%"
      >
        <div class="box-slider">
          <div class="text-header text-h3">
            <span>Rabat {{ percent }}%</span> na<br> pierwsze zamówienie!
          </div>
          <div class="text">
            Do 20 stycznia złóż zamówienie na stronie i skorzystaj z <b>promocji -10%.</b> Spiesz się, czas trwania
            promocji do
            końca lutego.
          </div>
          <v-btn
              color="#920303"
              class="btn text-white"
              width="160"
          >
            Zamów online
          </v-btn>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>

</template>

<script>
export default {
  name: "Slider",
  data() {
    return {
      percents: [
        '10',
        '10',
        '10'
      ],
    }
  },
}
</script>

<style lang="scss">

.box-slider {
  margin-left: 8vw;
  margin-top: 6vh;

  .text-header span {
    background-color: black;
    color: white;
  }

  .text {
    margin-top: 2vh;
    width: 350px;
  }

  .btn {
    margin-top: 1.8vh;
  }

}
</style>
