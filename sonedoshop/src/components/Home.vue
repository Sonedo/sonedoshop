<template>
  <div>
    {{ homeText }}
    <SliderMain style="width: 600px; height: 400px; align-items: center"/>
  </div>
</template>

<script>
  import SliderMain from './slider/SliderMain'
  export default {
    data() {
      return {
        homeText: 'Home Component'
      };
    },
    components: {
      SliderMain
    }
  };

</script>
