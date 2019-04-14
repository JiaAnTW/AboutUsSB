<template>
  <div class="self" v-bind:style="move" >
    <img id=background_03 src="../assets/About_us_03.png" alt="Pro_background">
    <div id="container">
      <Profile />
    </div>
  </div>
</template>

<script>
/* eslint-disable */
import Profile from './Profile.vue'
export default {
  name: 'selfIntro',
  props:['now'],
  data () {
    return {
      move:{
        left:'100%'
      },
      introduction:[
        {id:0,intro:"hi"},
        {id:1,intro:"hi"},
        {id:2,intro:"hi"},
        {id:3,intro:"hi"},
        {id:4,intro:"hi"}
      ],
      image: ["../assets/IMG_7963.jpg","../assets/IMG_7964.jpg","../assets/IMG_7966.jpg","../assets/IMG_7967.jpg","../assets/IMG_7968.jpg"],
    }
},
  components: {Profile},
  watch:{
  now:function(){
  console.log("test")
  if(this.now===3){
  const slide=()=>{
    this.move={left:'0%'}
    }
    slide();
    }
  }
  }
 } 
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
   .self{
      top:0rem;
      height:46.9rem;
      width: 100rem;
      max-width: 100%;
      background-color: rgb(232, 199, 103);
      position:absolute;
      -webkit-transition: left 1s ease-in-out;
      -moz-transition: left 1s ease-in-out;
      -o-transition: left 1s ease-in-out;
      transition: left 1s ease-in-out;
   }
  #background_03{
    position: absolute;
    margin-top: 0;
    margin-left: 7.5rem;
    height:46.9rem;
  }
  #container{
    position: absolute;
    top:0rem;
    left: 7.5rem;
    
  }
</style>