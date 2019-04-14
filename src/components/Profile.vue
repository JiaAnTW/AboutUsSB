
<template>

<div class="profile" >

<div id="mem_one"></div>
<div id="mem_two"></div>
<div id="mem_thr"></div>
<div id="mem_fou"></div>
<div id="mem_fiv"></div>
<div id="txt_one">
member_1
00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
</div>

</div>
</template>

<script>
/* eslint-disable */
export default {
name: 'profile',
props: ['image'],
data () {
return {
}
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.profile{
margin-top:10rem;
}

#mem_fiv
{
 left:69.32rem;
 position:absolute;
 width:10.85rem;
 height:10.85rem;
 top:19.43rem;
 background-image:url("../assets/About_us_01.png");
 background-position:center center;
 background-size:9rem auto;
 border-radius:10rem;
}

#mem_fou
{
 left:53.03rem;
 position:absolute;
 width:10.85rem;
 height:10.85rem;
 top:19.43rem;
 background-image:url("../assets/About_us_01.png");
 background-position:center center;
 background-size:9rem auto;
 border-radius:10rem;
}

#mem_thr
{
 left:36.37rem;
 position:absolute;
 width:10.85rem;
 height:10.85rem;
 top:19.43rem;
 background-image:url("../assets/About_us_01.png");
 background-position:center center;
 background-size:9rem auto;
 border-radius:10rem;
}

#mem_two
{
left:19.735rem;
position:absolute;
width:10.85rem;
height:10.85rem;
top:19.43rem;
background-image:url("../assets/About_us_01.png");
background-position:center center;
background-size:9rem auto;
border-radius:10rem;
}

#mem_one
{
left:3.28rem;
position:absolute;
width:10.85rem;
height:10.85rem;
top:19.43rem;
background-image:url("../assets/About_us_01.png");
background-position:center center;
background-size:9rem auto;
border-radius:10rem;
}

#txt_one
{
float: right;
}

span{
position: absolute;
margin-top: 1rem;
}

</style>
