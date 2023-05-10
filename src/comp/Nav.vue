<template>
    <v-card
      color="grey lighten-4"
      flat
      tile
    >
    
      <v-toolbar dense height="60">

<!-- Logo start         -->
        <div class="d-sm-center col">
          <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="d-sm-block d-md-none"> </v-app-bar-nav-icon>
          <v-toolbar-title class="d-flex d-sm-none d-md-flex">LOGO</v-toolbar-title>
        </div>
<!-- Logo End         -->


<!-- Middle Links Start -->

        <div class="d-flex justify-center col ">
        <div class="d-flex d-sm-block justify-center d-md-none">
          <v-toolbar-title>LOGO</v-toolbar-title>
        </div>

        <div class='d-sm-none d-md-flex'>
          <div class="pa-5">
            <a>STATIONARY</a>
          </div>

          <div class="pa-5">
            <a>WEDDING</a>  
          </div>

          <div class="pa-5">
            <a>BUSINESS</a>
          </div >

          <div class="pa-5">
            <a>HOLIDAY</a>
          </div>

          <div class="pa-5">
            <a>EVENTS</a>
          </div>
        </div>

      </div>

<!-- Middle Links End -->

<!-- Last Icons Start -->
<div class="d-flex justify-end col">
        <v-btn icon>
          <v-icon class="d-sm-none d-md-flex">mdi-magnify</v-icon>
        </v-btn>
  
        <v-btn icon>
          <v-icon class="d-sm-none d-md-flex">mdi-dots-vertical</v-icon>
        </v-btn>
  
        <v-btn icon>
          <v-icon>mdi-heart</v-icon>
        </v-btn>
</div>
<!-- Last Icons End -->

      </v-toolbar>
    </v-card>    
    
  </template>

<script>

export default{
    name:"NavVue",

    // data: () => ({
    //   drawer: false,
    //   group: null,
    // }),

    // watch: {
    //   group () {
    //     this.drawer = false
    //   },
    // },

  }

</script>

<style>

</style>