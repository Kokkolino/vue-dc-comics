<template>
  <div id="app">
    <HeaderComp/>
    <MainComp/>
    <FooterComp/>
  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
  }
}
</script>

<style lang="scss">
  @import "./assets/style/var.scss";

  #app {
    font-family: sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    height: 100vh;
    width: 100%;
  }

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: white;
  }

  .height-row{
    height: $hs;
  }

  .flex-bw{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .f-wrap{
    flex-wrap: wrap;
  }

  .flex-align{
    display: flex;
    align-items: center;
    justify-content: flex-start;
  }

  .h-100{
    height: 100%;
  }

  ul{
    list-style: none;
  }

  .horizontal-ul{
    display: flex;
  }

  .container-70{
    width: 70%;
    margin: auto;
  }
</style>