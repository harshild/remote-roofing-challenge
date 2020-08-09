<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
  import Header from "@/components/Header";

  export default {
    name: 'PageHeader',
    components: {
      Header
    }
  }
</script>

<style>
  @font-face {
    font-family: 'AirbnbCerealLight';
    src: url('https://uploads-ssl.webflow.com/5f127ac8860f158e650f06b5/5f129663d13f49d2bead206e_AirbnbCerealLight.woff') format('woff');
    font-weight: 300;
    font-style: normal;
  }
  #app {
    font-family: AirbnbCerealBold, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #fff;
  }
</style>
