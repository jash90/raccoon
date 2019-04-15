<template>
<div>
  <FirstSlide />
  <About />
  <Technology />
  <Price />
  <Slider />
</div>
</template>

<script>
  import FirstSlide from '../components/FirstSlide'
  import About from '../components/About'
  import Technology from '../components/Technology'
  import Price from '../components/Price'
  import Slider from '../components/Slider'

  export default {
    components: {
      FirstSlide,
      About,
      Technology,
      Price,
      Slider
    }
  }
</script>
