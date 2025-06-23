<template>
  <HeaderComponent/>

  <!-- <img class="banner" :src="logoSrc" alt="nStore Logo" style="width: 100%; height: 452px"/> -->
   <BannerComponent/>
   <onesolution/>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderComponent from './components/HeaderComponent.vue';
import BannerComponent from './components/BannerComponent.vue';
import onesolution from './components/onesolution.vue';


export default {
    components: { HeaderComponent,BannerComponent },
    data() {
    return {
      // logoSrc: require('@/assets/banner.png'),
    };
  },
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;ets
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */

  body, html {
  margin: 20px;
  padding: 0;
  overflow-x: hidden; /* Prevent horizontal overflow */
  width: 100%;
  height: 100%;
}

.container {
  max-width: 100%;
  overflow-x: hidden;
  box-sizing: border-box;
}

.banner{
  margin-top: 100px;
  /* margin: 20px; */
}

</style>
