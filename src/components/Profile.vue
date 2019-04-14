
<template>

<div class="profile" >

<div id="mem_one"></div>
<div id="mem_two"></div>
<div id="mem_thr"></div>
<div id="mem_fou"></div>
<div id="mem_fiv"></div>
<div id="h1-container">
  <h1 v-for="intro in introduction" :key="intro.name">{{intro.name}}</h1>
</div>
<div id="h2-container">
  <h2 v-for="intro in introduction" :key="intro.maj">{{intro.maj}}</h2>
</div>
<div id="span-container">
  <span v-for="intro in introduction" :key="intro.des">{{intro.des}}</span>
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
    introduction:[
      { name: "張家銨", maj:"資訊系 大二" ,des:"在2019年4月，他遇到了組員不交自我介紹的冏境，是進入大學後最難解的危機。"},
      { name: "楊子佑", maj:"電機系 大二" ,des:"哪種職業最安全?\n零售商。"},
      { name: "吳宜庭", maj:"工設所 ??" ,des:"宣稱在美國，就連小學生都能說一口流利的美語。"},
      { name: "許展境", maj:"電機系 大二" ,des:"他發現，NBA在2018-2019年，所有球隊的總勝率恰為5成。"},
      { name: "李立恆", maj:"電機系 大二" ,des:"根據他的研究，地球上超過8成的人，其父母恰在同一天結婚。"},
    ]

  }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css?family=Noto+Sans+TC:100,300,400,500');
#h1-container{
  font-family: 'Noto Sans TC';
  position: absolute;
  left: -5.3rem;
  width: 95rem;
  top: 30rem;
}
#h2-container{
  font-family: 'Noto Sans TC';
  position: absolute;
  left: -5rem;
  width: 95rem;
  top: 35.2rem;
}
#span-container{
  font-family: 'Noto Sans TC';
  position: absolute;
  left: -2.6rem;
  width: 95rem;
  top: 38rem;
}

h1{
  float: left;
  font-family: 'Noto Sans TC';
  font-weight: 400;
  color: rgb(41, 42, 44);
  padding-left: 10.6rem;
  
}

h2{
  float: left;
  font-family: 'Noto Sans TC';
  margin-top: -1rem;
  font-weight: 300;
  font-size: 1.3rem;
  color: rgb(41, 42, 44);
  padding-left: 9.6rem;
  text-align: center;
  width: 7rem;
}

span{
  float: left;
  font-family: 'Noto Sans TC';
  margin-top: -1rem;
  font-weight: 300;
  font-size: 1rem;
  color: rgb(41, 42, 44);
  padding-left: 5.7rem;
  text-align: center;
  width: 10.85rem;
}

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
 background-image:url("../assets/IMG_7970.png");
 background-position:center center;
 background-size:17rem auto;
 border-radius:10rem;
}

#mem_fou
{
 left:53.03rem;
 position:absolute;
 width:10.85rem;
 height:10.85rem;
 top:19.43rem;
 background-image:url("../assets/IMG_7969.png");
 background-position:center center;
 background-size:17rem auto;
 border-radius:10rem;
}

#mem_thr
{
 left:36.37rem;
 position:absolute;
 width:10.85rem;
 height:10.85rem;
 top:19.43rem;
 background-image:url("../assets/IMG_7968.png");
 background-position:center center;
 background-size:17rem auto;
 border-radius:10rem;
}

#mem_two
{
left:19.735rem;
position:absolute;
width:10.85rem;
height:10.85rem;
top:19.43rem;
background-image:url("../assets/IMG_7964.png");
background-position:center center;
background-size:17rem auto;
border-radius:10rem;
}

#mem_one
{
left:3.28rem;
position:absolute;
width:10.85rem;
height:10.85rem;
top:19.43rem;
background-image:url("../assets/IMG_7963.png");
background-position:center center;
background-size:17rem auto;
border-radius:10rem;
}

#txt_one
{
float: right;
}

</style>
