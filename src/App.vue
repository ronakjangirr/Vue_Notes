<template>
  <v-app>

    <v-main>
      <!-- <HelloWorld/> -->
      <!-- <ContainerVue /> -->
      <!-- <Flex /> -->
      <!-- <h2>{{ fun() }}</h2> -->

      <!-- <NavVue />
      <Nav2Vue />
      <BreadCrumbs />
      <HeroVue />
      <MiddleVue />
      <BeforeFooterVue />
      <FooterVue /> -->
      <AllcompNotes />
    </v-main>

  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld';
// import NavBar from './components/NavBar.vue';
// import ContainerVue from './components/Container.vue';


// Dummy Website ---
// import Nav2Vue from './comp/Nav2.vue';
// import NavVue from './comp/Nav.vue';
// import BreadCrumbs from './comp/BreadCrumbs.vue';
// import HeroVue from './comp/Hero.vue';
// import BeforeFooterVue from './comp/BeforeFooter.vue';
// import FooterVue from './comp/Footer.vue';
// import MiddleVue from './comp/Middle.vue';


// Vue Notes ---
import AllcompNotes from './vuenotes/AllcompNotes.vue';
// import Flex from './vuenotes/Flex.vue';


export default {
  name: 'App',

  components: {
    // NavVue,
    // Nav2Vue,
    // BreadCrumbs,
    // HeroVue,
    // MiddleVue,
    // BeforeFooterVue,
    // FooterVue
    AllcompNotes
  },

  data: function () {
    //   return{
    //     x : 10
    // }
    /// in data we can put or write our any variables and can access through this.x in functions

  },


  methods: {
    // fun()
    // {
    //   let a= this.x
    //   console.log(a);
    // }
  }
}
</script>
