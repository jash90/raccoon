<template>
  <v-content style="background-color: white">
    <v-layout
      class="general"
      text-xs-left
    >

      <v-flex xs6 class="img_box">
        <v-img
          :src="require('../assets/Logo_transparent.svg')"
          width="370"
          height="370"
        ></v-img>
      </v-flex>

      <v-flex xs6 class="text_block">
        <h3 class="mb-3" style="font-weight: 400; font-size: 22px;">
          O nas
        </h3>
        <p class="subheading font-weight-regular">
          <span v-for="item in 40">LOREM LOREM </span>
        </p>
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
  /* height: 542px; */
}

.text_block{
  margin-top: -4px;
  margin-left: 85px;

  max-width: 450px;
}


.img_box {
  background-color: #00ADEE;
  max-width: 370px;
  margin-left: 170px;
  height: 370px;
  /* margin-top: -50px; */
}
</style>
