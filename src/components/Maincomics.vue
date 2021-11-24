<template>
<div id="black">
    <div class="container">
      <div class="content">Content goes here</div>
    </div>
</div>
  
</template>

<script>
export default {
  name: 'Main',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#black {
    display: flex;
    align-items: center;
    height: 100px;
    background-color: black;
    color: white;
    .container{
        width: 80%;
        margin: 0 auto;
    }
    
}
</style>