<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
    <OnGoingSeries/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';
import OnGoingSeries from './components/OnGoingSeries.vue';
export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
    OnGoingSeries
  }
}
</script>

<style lang="scss">
  @import "./assets/style/general.scss"; 
</style>