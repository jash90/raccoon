<template>
  <v-content style="background-color: #F5F5F5">
    <v-layout
      class="general"
      text-xs-center
    >

      <v-flex xs12 class="text_block">
        <h3 class="mb-3" style="font-weight: 400; font-size: 22px;">
          Technologie
        </h3>
        <p class="subheading font-weight-regular">

          <span v-for="item in 40">LOREM LOREM </span>
          
        </p>
      </v-flex>
    </v-layout>

    <v-layout
        text-xs-center
        align-center justify-center row
        class="more_img_box"
      >
        <v-flex xs3 class="img_box">
          <v-img
            :src="require('../assets/apple.svg')"
            width="200"
            height="200"
          ></v-img>
        </v-flex>
        <v-flex xs3 offset-xs1 class="img_box">
          <v-img
            :src="require('../assets/android.svg')"
            width="200"
            height="200"
          ></v-img>
        </v-flex>
        <v-flex xs3 offset-xs1 class="img_box">
          <v-img
            :src="require('../assets/Web.svg')"
            width="200"
            height="200"
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
  /* height: 542px; */
}

.text_block{
  margin-top: -60px;
  margin-left: 160px;

  max-width: 900px;
}


.img_box {
  /* max-width: 400px; */
  /* margin-left: 200px; */
  /* height: 200px; */
  /* margin-top: -50px; */
}

.more_img_box {
  padding: 0px 200px;
  margin: auto;
  max-width: 1200px;
  height: 220px;
}
</style>
