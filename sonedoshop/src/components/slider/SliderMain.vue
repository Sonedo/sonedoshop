<template>
  <div class="slider-main">
    <div style="width: 600px; height: 400px; background-color: blue"></div>
    <div style="width: 600px; height: 400px; background-color: aqua"></div>
    <div style="width: 600px; height: 400px; background-color: brown"></div>
  </div>
</template>

<script>
  export default {
    name: "SliderMain",
    mounted() {
      global.$('.slider-main').slick()
    }
  }

</script>

<style scoped>

</style>
