<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div>
      <ul>
        <li>CHARACTERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  margin: 0 auto;
  height: 100px;
  img {
    height: 75px;
  }
  ul{
    margin-right: 30px;
    display: flex;
    list-style: none;
    li{
      margin: 15px;
    }
  }
}
</style>