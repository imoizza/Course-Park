/* eslint-disable */ 
<template>
  <div id="app">
     <router-view />
  </div>
</template>

<script>
export default {
  name: "app",
  mounted(){
    this.$store.dispatch('GetCourses');
    this.$store.dispatch('GetDepartments');
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

*{
  padding:0;
  margin:0;
  box-sizing:border-box;
  scroll-behavior: smooth;
    --webkit-font-smoothing: antialiased;
}

/* The basic color pallete for the application */
:root {
  --primary: #FFCC00;
  --dark: #1D1D1D;
  --ternary: #303030;
  --secondary: #999999;
  --light: #F2F2F2;
  --pure: #FFFFFF;
}
</style>
