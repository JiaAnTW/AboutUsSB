<template>
  <div class="team" v-bind:style="fly">
    <img id="background_02" src="../assets/About_us_02.png" alt="background_02"/>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'team',
  props: ['now'],
  data () {
    return {
      fly:{
        left:'-100rem', 
      },
    }
  },
  watch:{
    now:function(){
      if(this.now===2){
        const flyin=()=>{
          this.fly={left:'0'}
        }
        setTimeout(flyin,1000);
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .team{
    position:absolute;
    height:46.9rem;	
		-webkit-transition:  left  1s ease-in-out;
    -moz-transition:  left  1s ease-in-out;
    -o-transition: left  1s ease-in-out;
    transition: left 1s ease-in-out;
		
  }
  #background_02{
    position:absolute;
    margin-top:0;
    height:46.9rem;
    width:100rem;
	}
</style>
