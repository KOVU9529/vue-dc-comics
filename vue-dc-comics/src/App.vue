<template>
  <div id="app">
    <HeaderComp />
    <MainComp/>
    <DcList />
    <MainComp2 />
    <FooterEnd />
    <FooterEnd2 />

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import DcList from './components/DcList.vue';
import MainComp2 from './components/MainComp2.vue';
import FooterEnd from './components/FooterEnd.vue';
import FooterEnd2 from './components/FooterEnd2.vue';

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    DcList,
    MainComp2,
    FooterEnd,
    FooterEnd2
  }
}
</script>

<style lang="scss">

 @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;1,300&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Roboto', sans-serif;
}

</style>
