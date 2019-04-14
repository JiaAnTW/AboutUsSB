<template>
  <div class="view">
    <self-intro @change-now-at="handleChangeNowAt" :now="nowAt"/>
    <team @change-now-at="handleChangeNowAt" :now="nowAt"/>
    <landing @change-now-at="handleChangeNowAt" :now="nowAt"/>
  </div>
</template>

<script>
/* eslint-disable */
import Landing from './components/Landing.vue'
import Team from './components/Team.vue'
import SelfIntro from './components/SelfIntro.vue'
export default {
  name: 'Index',
  components: {Landing,Team,SelfIntro},
  data () {
    return {
      nowAt: 1,
    }
  },
  methods:{
    handleChangeNowAt: function(page){
      this.nowAt=page;
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
    height: 46.8rem;
    
  }

</style>
