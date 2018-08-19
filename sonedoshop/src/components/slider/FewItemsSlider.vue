<template>
    <div class="few-items-slider">
      <div><img src="../../assets/img/img1.jpg"/></div>
      <div><img src="../../assets/img/img2.jpg"/></div>
      <div><img src="../../assets/img/img3.jpg"/></div>
      <div><img src="../../assets/img/img4.jpg"/></div>
      <div><img src="../../assets/img/img5.jpg"/></div>
      <div><img src="../../assets/img/img6.jpg"/></div>
      <div><img src="../../assets/img/img3.jpg"/></div>
      <div><img src="../../assets/img/img4.jpg"/></div>
    </div>
</template>

<script>
    export default {
        name: "FewItemsSlider",
      mounted() {
        $('.few-items-slider').slick({
          dots: true,
          infinite: true,
          speed: 300,
          slidesToShow: 6,
          slidesToScroll: 1,
          responsive: [
            {
              breakpoint: 1024,
              settings: {
                slidesToShow: 4,
                slidesToScroll: 1,
                infinite: true,
                dots: true
              }
            },
            {
              breakpoint: 800,
              settings: {
                slidesToShow: 3,
                slidesToScroll: 1
              }
            },
            {
              breakpoint: 550,
              settings: {
                slidesToShow: 2,
                slidesToScroll: 1
              }
            }
          ]
        });
      }
    }
</script>

<style scoped>
  .few-items-slider {
    height: 150px;
    max-width: 900px;
    margin-top: 30px;
    margin-left: 30px;
  }
  @media (max-width: 1024px) {
    .few-items-slider{
      max-width: 600px;
    }
  }
  @media (max-width: 800px) {
    .few-items-slider{
      max-width: 450px;
    }
  }
  @media (max-width: 550px) {
    .few-items-slider{
      max-width: 300px;
    }
  }
</style>
