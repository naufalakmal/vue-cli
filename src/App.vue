<template>
  <div id="container">
    <nav>
      <!-- directive untuk membuat link tautan antar component -->
      <!-- <router-link to="/">Home | </router-link>
      <router-link to="/about">About</router-link> -->
      <!-- Named Routes klo misal ada yg diubah gausah ganti kya yg diatas-->
      <router-link :to="{name: 'Home'}">Home</router-link> |
      <router-link :to="{name: 'About'}">About</router-link> |
      <router-link to="/user/Akmal">User</router-link>
    </nav>

<!-- pada saat route navigasi di akses otomatis router view akan dirender -->
    <router-view></router-view>
  </div>
</template>

<script>

export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
