<template>
  <div class="landing" v-bind:style="clip">
    <img id="background_01" src="../assets/About_us_01.png" alt="background_01"/>
    <button class="circle_btn" v-on:click="small"></button>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name: 'landing',
  props: ['now'],
  data () {
    return {
      clip: {
        clipPath: 'circle(100% at 50% 50%)',
        WebkitClipPath: 'circle(100% at 50% 50%)',
        display: "block",
      },
  }
},
  methods: {
    small: function(event){
      const smaller =()=> {
        this.clip={clipPath: 'circle(0% at 61% 64%)',WebkitClipPath: 'circle(0% at 61% 64%)',display: "block"};
      }
      smaller();
      this.$emit('change-now-at',2);
      const emerge =()=>{
        this.clip={clipPath: 'circle(0% at 61% 64%)',WebkitClipPath: 'circle(0% at 61% 64%)',display: "none"};
      }
      setTimeout(emerge,1500);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #background_01{
    position: absolute;
    margin-top: 0 ;
    margin-left: 13rem;
    height: 46.9rem;
    width: auto;
  }
  .landing{
    margin-top: 0 ;
    margin-left: 0;
    width: 100rem;
    max-width: 100%;
    height: 46.9rem;
    overflow:hidden;
    display: inline-block;
    background-color: rgb(235, 195, 91);
    -webkit-transition: clip-path 1.5s ease-in-out;
    -moz-transition: clip-path 1.5s ease-in-out;
    -o-transition: clip-path 1.5s ease-in-out;
    transition: clip-path 1.5s ease-in-out;
  }
  .circle_btn{
    position: absolute;
    left: 51rem;
    top: 21rem;
    width: 18.5rem;
    height: 20rem;
    border-radius: 18.5rem;
    background-color:rgba(243,243,243,0);
    border: none;
    outline: none;
  }
</style>