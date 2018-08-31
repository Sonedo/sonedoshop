<template>
  <div id="app">
    <AppHeader/>
    <router-view></router-view>
  </div>
</template>
<script>
  import AppHeader from './components/header/AppHeader.vue'
  export default {
    beforeMount() {
      global.$ = require('jquery');
      global.slickCarousel = require('slick-carousel');
      global.materializeCss = require('materialize-css/')
    },
    components:{
      AppHeader
    }
  };
</script>
