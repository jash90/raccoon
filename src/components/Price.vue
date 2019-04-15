<template>
  <v-content style="background-color: white">
    <v-layout
      class="general"
      text-xs-left
    >
      <v-flex xs3 offset-xs1 class="img_box">
          <v-img
            :src="require('../assets/android.svg')"
            width="200"
            height="200"
          ></v-img>
        </v-flex>

      <v-flex xs9 class="text_block">
        <h3 class="mb-3" style="font-weight: 400; font-size: 22px;">
          Wycena aplikacji
        </h3>
        <p class="subheading font-weight-regular">

          <!-- <span v-for="item in 40">LOREM LOREM </span> -->
          <v-form
            ref="form"
            v-model="valid"
            lazy-validation
          >
            <!-- <v-layout align-center justify-center row fill-height> -->
              <v-radio-group v-model="row" row>
                Rodzaj aplikacji: 
                <v-radio label="Strona" value="radio-1" style="margin-left: 35px;"></v-radio>
                <v-radio label="Aplikacja" value="radio-2"></v-radio>
                <v-radio label="Strona i aplikacja" value="radio-3"></v-radio>
              </v-radio-group>
            <!-- </v-layout> -->

            <v-text-field
              class="custom_btn"
              v-model="name"
              :rules="[v => !!v || 'To pole jest wymagane!']"
              label="Funkcjonalności"
              outline
              required
            ></v-text-field>
            <v-textarea
              class="custom_btn"
              v-model="name"
              :rules="[v => !!v || 'To pole jest wymagane!']"
              label="Opis"
              outline
            ></v-textarea>

            Kontakt:

            <v-text-field
              v-model="email"
              :rules="[v => !!v || 'To pole jest wymagane!']"
              label="Imię i nazwisko"
              outline
              required
            ></v-text-field>

            <v-text-field
              class="custom_btn"
              v-model="email"
              :rules="[v => !!v || 'To pole jest wymagane!']"
              label="E-mail"
              outline
              required
            ></v-text-field>


            <v-btn
              :disabled="!valid"
              color="success"
              @click="validate"
            >
              WYŚLIJ!
            </v-btn>
          </v-form>
          
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
  max-width: 900px;
  margin: auto;
  padding-bottom: 100px;
  /* height: 542px; */
}

.text_block{
  margin-top: -60px;
  margin-left: 10px;

  max-width: 900px;
}

.custom_btn{
  border-radius: 0px !important;
  margin-top: -25px;
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
