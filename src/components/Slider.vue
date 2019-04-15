<template>
  <v-content style="background-color: #00ADEE">
    <v-layout
      class="general"
      text-xs-center
    >

      <v-flex xs12 class="text_block">
        <h3 class="mb-3" style="font-weight: 400; font-size: 22px;">
          DBAMY O NASZYCH KLIENTÓ
        </h3>
        <p class="subheading font-weight-regular">

          <span v-for="item in 20">LOREM LOREM </span>
          
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
  margin: auto;

  max-width: 500px;
}

</style>
