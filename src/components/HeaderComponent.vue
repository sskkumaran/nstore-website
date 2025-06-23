<template>
  <header>
    <div
    style="width: 2500px; height: 60px; justify-content: flex-start; align-items: flex-end; gap: 451px; top: 0px;  display: inline-flex">
    <!-- <img style="width: 162px; height: 52px" src="https://via.placeholder.com/162x52" /> -->
    <!-- <img src="./assets/nStore.png" alt="img" style="width: 162px; height: 52px"> -->
    <img :src="logoSrc" alt="nStore Logo" style="width: 162px; height: 52px"/>
    <div style="justify-content: flex-start; align-items: center; gap: 26px; top: 46px; display: flex">
      <div style="color: #2288B2; font-size: 16px; font-family: Ubuntu; font-weight: 400; word-wrap: break-word">Home </div>
      <div style="color: #747582; font-size: 16px; font-family: Ubuntu; font-weight: 400; word-wrap: break-word">About us</div>
      <div style="color: #747582; font-size: 16px; font-family: Ubuntu; font-weight: 400; word-wrap: break-word">Platforms</div>
      <div style="color: #747582; font-size: 16px; font-family: Ubuntu; font-weight: 400; word-wrap: break-word">Career</div>
      <div style="color: #747582; font-size: 16px; font-family: Ubuntu; font-weight: 400; word-wrap: break-word">Contact Us</div>
      <div
        style="width: 143px; height: 42px; padding-left: 24px; padding-right: 24px; padding-top: 13px; padding-bottom: 13px; background: white; border-radius: 80px; border: 1px rgba(255, 105.19, 141.05, 0.50) solid; justify-content: center; align-items: center; gap: 10px; top:46px; display: flex">
        <div style="color: #282C4B; font-size: 14px; font-family: Ubuntu; font-weight: 700; word-wrap: break-word">Buy
          on ONDC</div>
      </div>
      <div
        style="width: 143px; height: 42px; padding-left: 25px; padding-right: 25px; padding-top: 13px; padding-bottom: 13px; background: white; border-radius: 80px; border: 1px rgba(255, 105.19, 141.05, 0.50) solid; justify-content: center; align-items: center; gap: 10px; display: flex">
        <div style="color: #282C4B; font-size: 14px; font-family: Ubuntu; font-weight: 700; word-wrap: break-word">Sell
          on ONDC</div>
      </div>
    </div>
  </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderComponent',
  data() {
    return {
      logoSrc: require('@/assets/nStore.png'),
    };
  },
};
</script>

<style scoped>
/* Basic styling for the header */
header {
  background-color: #fff;
  border-bottom: 1px solid #ddd;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 10px 0;
}

/* Container for centering and spacing */
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Logo styling */
.logo {
  font-size: 24px;
  font-weight: bold;
  color: #333;
}

/* Navigation styling */
nav ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

nav li {
  margin-left: 20px;
}

nav a {
  text-decoration: none;
  color: #333;
  font-weight: 500;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #007BFF;
}

/* Responsive design for mobile view */
@media (max-width: 768px) {
  .container {
    flex-direction: column;
    align-items: flex-start;
  }

  nav ul {
    flex-direction: column;
    width: 100%;
  }

  nav li {
    margin-left: 0;
    margin-top: 10px;
  }
}
</style>
