<template>
  <v-carousel
      cycle
      height="450"
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
        <div class="text">
          <div class="text-first text-h3">
            <span>Rabat {{ percent }}%</span> na<br> pierwsze zamówienie!
          </div>
          <div class="text-second">
            Do 20 stycznia złóż zamówienie na stronie i skorzystaj z <b>promocji -10%.</b> Spiesz się, czas trwania
            promocji do
            końca lutego.
          </div>
          <v-btn
              color="#920303"
              class="btn text-white"
              width="160"
          >
            Zamów oline
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

.text {
  margin-left: 8vw;
  margin-top: 7vh;

  .text-first span {
    background-color: black;
    color: white;
  }

  .text-second {
    margin-top: 2vh;
    width: 350px;
  }

  .btn {
    margin-top: 2vh;
  }

}
</style>
