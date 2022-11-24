<template>
  <div>
    <nav class="height-row flex-bw container-70">
      <!-- logo -->
      <img src="../assets/dc-logo.png" alt="">
      <!-- nav btn -->
      <ul class="horizontal-ul">
        <li>
          CHARACTERS
          <span class="line-dec"></span>
        </li>
        <li>
          COMICS
          <span class="line-dec"></span>
        </li>
        <li>
          MOVIES
          <span class="line-dec"></span>
        </li>
        <li>
          TV
          <span class="line-dec"></span>
        </li>
        <li>
          GAMES
          <span class="line-dec"></span>
        </li>
        <li>
          COLLECTIBLES
          <span class="line-dec"></span>
        </li>
        <li>
          VIDEOS
          <span class="line-dec"></span>
        </li>
        <li>
          FANS
          <span class="line-dec"></span>
        </li>
        <li>
          NEWS
          <span class="line-dec"></span>
        </li>
        <li>
          SHOP
          <span class="line-dec"></span>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
  export default {
    name: 'HeaderComp',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  div{
    background-color: white;
    z-index: 2;
  }

  nav{
    margin: auto;
  }
  
  li{
    position: relative;
    margin: 0 15px;
    font-size: 13px;
    color: black;
  }

  li:hover{
    cursor: pointer;
    color: blue;
    .line-dec{
      display: block;
    }
  }


  .line-dec{
    display: none;
    bottom: -52px;
    right: 0;
    position: absolute;
    width: 100%;
    height: 4px;
    background-color: blue;
  }
</style>
