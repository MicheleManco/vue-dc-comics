<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div>
      <ul>
        <li :class="link.status ? 'active' : ''" v-for="link,i in links" :key="i">
          <a href="">{{link.text}}</a> 
          </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
        return{
            links:[
                {
                text: "CHARACTERS",
                status: true 
                },
                {
                text: "COMICS",
                status: false  
                },
                {
                text: "MOVIES",
                status: false  
                },
                {
                text: "TV",
                status: false 
                },
                {
                text: "GAMES",
                status: false 
                },
                {
                text: "COLLECTIBLES",
                status: false 
                },
                {
                text: "VIDEOS",
                status: false  
                },
                {
                text: "FANS",
                status: false  
                },
                {
                text: "NEWS",
                status: false 
                },
                {
                text: "SHOP",
                status: false  
                },
               
            ]
        }
    }
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
      line-height: 95px;
      margin: 15px;
       &.active a{

            border-bottom: 5px solid rgb(0, 110, 255);
            color: rgb(0, 110, 255);
        }
      a{
        padding-bottom: 36px;
        color: black;
        text-decoration: none;
        
      }
     
    }
  }
}
</style>