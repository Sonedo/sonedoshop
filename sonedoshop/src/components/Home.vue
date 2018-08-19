<template>
  <div>
    {{ homeText }}
    <SliderMain style="width: 600px; height: 400px; align-items: center" v-cloak/>
    <FewItemsSlider v-cloak/>
  </div>
</template>

<script>
  import SliderMain from './slider/SliderMain'
  import FewItemsSlider from './slider/FewItemsSlider'
  export default {
    data() {
      return {
        homeText: 'Home Component'
      };
    },
    components: {
      SliderMain, FewItemsSlider
    }
  };

</script>
