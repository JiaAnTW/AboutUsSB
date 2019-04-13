<template>
  <div class="view">
    <Landing/>
  </div>
</template>

<script>
import Landing from './components/Landing.vue'
export default {
  name: 'Index',
  components: {Landing},
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .view{
    margin-top: 0 ;
    margin-left: 0;
    width: 100rem;
    max-width: 100%;
    height: 47rem;
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
