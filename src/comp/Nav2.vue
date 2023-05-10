<template>
    <div>

        <v-card
    class="mx-auto overflow-hidden"
  >
    <!-- <v-system-bar color="deep-purple darken-3"></v-system-bar> -->

    <v-app-bar
      color="deep-purple accent-4"
      dark
    >

    <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="d-flex"> </v-app-bar-nav-icon>
        
      <v-toolbar-title class="d-flex justify-end col">My files</v-toolbar-title>

      <div class="d-flex justify-end col">
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-filter</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </div>

    </v-app-bar>

    
  </v-card>    
  
  <v-navigation-drawer
      v-model="drawer"
      absolute
      bottom
      temporary
      class="d-sm-block"
    >
      <v-list
        nav
        dense
        class="d-sm-block"
      >
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
          class="d-sm-block"
        >
          <v-list-item  class="d-sm-block">
            <v-list-item-title>Foo</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Bar</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Fizz</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-title>Buzz</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>


  </div>
</template>

<script>
export default {
    name:"Nav2Vue",

    data: () => ({
      drawer: false,
      group: null,
    }),

    watch: {
      group () {
        this.drawer = false
      },
    },
}
</script>

<style>
</style>