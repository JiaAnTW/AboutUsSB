<template>
  <div class="landing">
    <img id="background_01" src="../assets/About_us_01.png" alt="background_01"/>
  </div>
</template>

<script>
export default {
  name: 'landing',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #background_01{
    position: relative;
    margin-top: 0 ;
    margin-left: 13rem;
    height: 47rem;
    width: auto;
    animation: Small 1.5s ;
  }
  .landing{
    margin-top: 0 ;
    margin-left: 0;
    width: 100rem;
    max-width: 100%;
    height: 47rem;
    overflow:hidden;
    display: inline-block;
    white-space:nowrap;
  }

  @keyframes Small {
    0% {
      -webkit-clip-path: circle(100% at 50% 50%);
      clip-path: circle(100% at 50% 50%);
    }
    100% {
      -webkit-clip-path: circle(0% at 69% 67%);
      clip-path: circle(0% at 69% 67%);
    }
  }
</style>
