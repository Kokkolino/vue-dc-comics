<template>
  <div>
    <nav class="height-row flex-bw container-70">
      <!-- logo -->
      <img src="../assets/dc-logo.png" alt="">
      <!-- nav btn -->
      <ul class="horizontal-ul">
        <li>
          CHARACTERS
        </li>
        <li>
          COMICS
        </li>
        <li>
          MOVIES
        </li>
        <li>
          TV
        </li>
        <li>
          GAMES
        </li>
        <li>
          COLLECTIBLES
        </li>
        <li>
          VIDEOS
        </li>
        <li>
          FANS
        </li>
        <li>
          NEWS
        </li>
        <li>
          SHOP
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
    margin: 0 15px;
    font-size: 13px;
    color: black;
  }

  li:hover{
    cursor: pointer;
  }
</style>
