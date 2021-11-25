<template>
<div>
    <div class="cont-card">
        <div class="img-card">
            <img :src="details.thumb" alt="">
        </div>
            
        <div>
            {{details.series}}
        </div>
    </div>
    
</div>
  
</template>

<script>
export default {
  name: 'Fumetto',
  props: {
      details: Object
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.cont-card {
    padding: 20px;
}
.img-card {
    height: 210px;
    overflow: hidden;
    margin-bottom: 15px;
}
img {
width: 100%;
}
</style>