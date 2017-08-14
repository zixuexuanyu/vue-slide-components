<template>
  <div id="app">
    <img src="./assets/logo.png">
    <slideshow :slides='slides' :inv="slideSpeed"></slideshow>
    <!-- <router-view></router-view> -->
  </div>
</template>

<script>
import slideshow from './components/layout'
export default {
  components:{
    slideshow
  },
  data () {
    return {
      slideSpeed: 2000,
      slides: [
        {
          src: require('./assets/images/1.jpg'),
          title: 'xxx1',
          href: 'detail/analysis'
        },
        {
          src: require('./assets/images/2.jpg'),
          title: 'xxx2',
          href: 'detail/count'
        },
        {
          src: require('./assets/images/3.jpg'),
          title: 'xxx3',
          href: 'http://xxx.xxx.com'
        },
        {
          src: require('./assets/images/4.jpg'),
          title: 'xxx4',
          href: 'detail/forecast'
        }
      ]
    }
  }
}
</script>

<style>

</style>
