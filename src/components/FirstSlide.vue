<template>
  <v-content style="background-color: #00ADEE">
    <v-layout
      class="general"
      text-xs-left
      align-center justify-center row fill-height
    >

      <v-flex xs6 class="text_block">
        <h1 class="display-2 mb-3" style="font-weight: 900;">
          RACCON SOFTWARE
        </h1>
        <p class="subheading font-weight-regular">
          Rozwiązujemy twoje problemy.
        </p>
        <v-btn depressed class="head_button"> KONTAKT </v-btn>
      </v-flex>

      <v-flex xs6>
        <v-img
          style="margin-left: -50px; margin-top: 0px;"
          :src="require('../assets/Logo_transparent.svg')"
          width="640"
          height="450"
        ></v-img>
      </v-flex>
    </v-layout>
  </v-content>
</template>

<script>
  export default {
    data: () => ({
      
    })
  }
</script>

<style scoped>
.general{
  max-width: 1200px;
  margin: auto;
  padding-bottom: 100px;
  height: 500px;
}

.text_block{
  margin-top: 25px;
  margin-left: 120px;
  color: white;
}

.head_button {
  margin-top: 30px; 
  width: 180px; 
  height: 45px; 
  margin-left: 0px;
  border-radius: 0px;
  color: #00ADEE;
}
</style>
