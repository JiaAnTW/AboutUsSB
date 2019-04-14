
<template>
  <div class="team" v-bind:style="move" >
    <img id=background_03 src="../assets/About_us_03.png" alt="Pro_background">
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'team',
  props:['now'],
  data () {
    return {
      move:{
        left:'100%'
      },
    }
},
  watch:{
  now:function(){
  console.log("test")
  if(this.now===3){
  const slide=()=>{
    this.move={left:'0%'}
    }
    setTimeout(slide,1000)
    }
  }
  }
 } 
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
   .self{
   height:46.9rem;
   }
   .team{
     position:absolute;
     width:100%;
      -webkit-transition: left 1s ease-in-out;
      -moz-transition: left 1s ease-in-out;
      -o-transition: left 1s ease-in-out;
      transition: left 1s ease-in-out;
   }
  #background_03{
  width:100%;
  }
</style>
