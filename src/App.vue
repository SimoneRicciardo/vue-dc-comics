<template>
  <div id="app">
      <MyHeader/>
      <MyMain/>
      <FooterTop/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import FooterTop from './components/FooterTop.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    FooterTop
}
}
</script>

<style lang="scss">

</style>
