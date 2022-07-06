<template>
  <div id="app">
    <HeaderComp />
    <MainComp />
    <MainComp2 />
    <FooterEnd />


  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import MainComp2 from './components/MainComp2.vue';
import FooterEnd from './components/FooterEnd.vue';


export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    MainComp2,
    FooterEnd
  }
}
</script>

<style lang="scss">
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

</style>
