<template>
    <div>
      <home-hearder></home-hearder>
      <home-swiper></home-swiper>
      <home-icons></home-icons>
    </div>
</template>

<script>
import HomeHearder from './components/Header'
import HomeSwiper from './components/Swiper'
import HomeIcons from './components/Icons'
export default {
  name: 'Home',
  components: {
    HomeHearder,
    HomeSwiper,
    HomeIcons
  }
}
</script>

<style>

</style>
