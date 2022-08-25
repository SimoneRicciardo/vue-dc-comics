<template>
  <div id="app">
      <MyHeader/>
      <MyMain/>
      <FooterTop/>
      <FooterBottom/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import FooterTop from './components/FooterTop.vue';
import FooterBottom from './components/FooterBottom.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    FooterTop,
    FooterBottom
}
}
</script>

<style lang="scss">

@import './style/container.scss';
@import './style/general.scss';

</style>
