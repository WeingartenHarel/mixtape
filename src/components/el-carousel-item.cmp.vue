<template>
  <section class="hero">
    {{item}}
  </section>
</template>

<script>
export default {
  name:'mix-el-carousel',
  data(){
    return{
      imgs:[
        'url',
        'url',
        'url',
        'url'
      ]
    }
  },
  props:{
   item:String
  },
  components: {

  },
  computed : {
  },
  created(){
    console.log('hero')
  }
}
</script>

<style>
  .el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    /* line-height: 200px; */
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
  }
</style>