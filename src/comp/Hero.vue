<template>
<v-container>
    <v-row >
        <v-col cols="8" class="d-flex bg_custom_hero align-center d-wrap pa-0">
            <div>
              <h1 class="text-uppercase px-12 pb-2 pa-0 h1 ls-n10 text-left brown--text align-center">
                Stationery
              </h1 >
              <p class="fontsize-16 line-height-18 pa-0 mt-md-2 mt-lg-2 body-font px-12 ls-n10 text-left brown--text">
                Send a traditional, handwritten note using custom stationery with carefully selected details and finishes to make each message feel truly special. Suitable for personal and professional occasions, our stationery shop instantly adds a unique touch to all your correspondence.
              </p>
            </div>
        </v-col>
        <v-col cols="4" class="pa-0" >
            <v-img
              src="../assets/HP-Block1-121922.jpg" 
              height="400"
              cover
              class="bg-grey-lighten-2"
            ></v-img>        
        </v-col>
    </v-row>
</v-container>
</template>

<script>
export default{
    name:"HeroVue",
}
</script>


<style>
.bg_custom_hero{
  background-color: #D7CCC8;
}
</style>