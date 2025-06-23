<template>
  <div :style="bannerStyle" class="banner">
   
  </div>
</template>

<script>
export default {
  name: 'BannerComponent',
  data() {
    return {
      bannerImageUrl: require('@/assets/banner.png') // Adjust the path to your image
    };
  },
  computed: {
    bannerStyle() {
      return {
        backgroundImage: `url(${this.bannerImageUrl})`,
        backgroundSize: 'cover',
        backgroundPosition: 'center',
        width: '100%',
        height: '650px'
      
      };
    }
  }
};
</script>

<style scoped>
.banner {
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
  padding-left:70px;
 /* background-color: rgba(0, 0, 0, 0.134);  Fallback color if the image fails to load */
}
</style>