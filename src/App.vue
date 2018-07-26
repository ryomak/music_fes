<template>
  <div id="app">
    <header-component/>
    <img src="./assets/logo.png">
    <top/>
    <footer-component/>
  </div>
</template>

<script>

import Top from '@/components/top/index'
import HeaderComponent from "@/components/layout/HeaderComponent"
import FooterComponent from "@/components/layout/FooterComponent"
export default {
  name: 'App',
  components:{
    HeaderComponent,
    Top,
    FooterComponent,
  }
}
</script>

<style scoped>

</style>
