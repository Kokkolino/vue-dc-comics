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
  #app {
    font-family: sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    color: white;
  }

  .height-row{
    height: 120px;
  }

  .flex-bw{
    display: flex;
    justify-content: space-between;
    align-items: center;
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
    display: flex;
  }

  .container-70{
    width: 70%;
    margin: auto;
  }
</style>