<template>
  <div class="team" v-bind:style="fly">
    <img id="background_02" src="../assets/About_us_02.png" alt="background_02"/>
    <button class="circle_btn" v-on:click="move"></button>
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
        left:'0', 
      },
    }
  },
  methods:{
    move:function(){
      this.$emit('change-now-at',3);
        const flyin=()=>{
          this.fly={left:'-100rem'}
      }
      flyin();
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .team{
    position:absolute;
    height:46.8rem;
    top: 0rem;
		-webkit-transition:  left  1s ease-in-out;
    -moz-transition:  left  1s ease-in-out;
    -o-transition: left  1s ease-in-out;
    transition: left 1s ease-in-out;
		
  }
  #background_02{
    position:absolute;
    margin-top:0;
    margin-left: 10rem;
    height:46.8rem;
    
	}
    .circle_btn{
    position: absolute;
    left: 76.7rem;
    top: 24.0rem;
    width: 2.9rem;
    height: 2.9rem;
    border-radius: 18.5rem;
    background-color:rgba(243,243,243,0);
    border: none;
    outline: none;
  }
</style>
