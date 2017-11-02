<template>
  <div id="head">
        <div class="fl">
            <img src="../../../static/images/logohead.png" >
        </div>
        <div class="fl">
            <ul>
                <li><a href="#">关注有礼</a></li>
                <li><a href="#">登录</a>|<a href="#">注册</a></li>
                <li><a href="#">收藏本站</a>|<a href="#">网站地图</a></li>
            </ul>
            <div class="clear phone">
                <span>省心 省钱 省事，互联网家装领导品牌</span>
                <span class="bgfont20 bgred">|400-888-6266</span>
            </div>
        </div>
        <div class="main_head   clear  textleft">
               <ul>
                   <li v-for='( item,index) in lists'><router-link :to="item.link" ><span :class='item.class' >{{item.title}}</span></router-link><span class="fr" >|</span></li>
                   <!-- <li><router-link to="zhengzhuang">整装套餐</router-link><span class="bgred fr">|</span></li>
                   <li><a href="#" >局部翻新</a><span class="bgred fr">|</span></li>
                   <li><a href="#" >软装配饰</a><span class="bgred fr">|</span></li>
                   <li><a href="#" >设计与报价</a><span class="bgred fr">|</span></li>
                   <li><a href="#" >效果图</a><span class="bgred fr">|</span></li>
                   <li><a href="#" >装修攻略</a><span class="bgred fr">|</span></li>
                   <li><a href="#" >百创实力</a><span class="bgred fr">|</span></li> -->
               </ul>
        </div>
  </div>
</template>
 <script>
export default {
data(){
  return{
    lists:[
      {title:'首页',link:'/',class:'bgred1'},
      {title:'整装套餐',link:'/zhengzhuang',class:'bgred2'},
      {title:'局部翻新',link:'#',class:'bgred3'},
      {title:'软装配饰',link:'#',class:'bgred4'},
      {title:'设计与报价',link:'#',class:'bgred5'},
      {title:'效果图',link:'#',class:'bgred6'},
      {title:'装修攻略',link:'#',class:'bgred7'},
      {title:'百创实力',link:'#',class:'bgred8'},
    ]
  }
},
  props:['istrue']
};
</script>
<style scoped>

#head {
  width: 100%;
  height: 1.22rem;
  font-size: 0.12rem;
  color: #7e7e7e;
}
a {
  color: #7e7e7e;
}
#head .fl {
  width: 50%;
  text-align: center;
}
.fl ul {
  height: 0.4rem;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  justify-content: center;
}
.fl ul li {
  float: left;
  line-height: 0.4rem;
  padding-left: 0.15rem;
}
.phone {
  padding-right: 0.8rem;
}
.main_head {
  width: 100%;
  height: 0.42rem;
}
.main_head ul {
  width: 100%;
  height: 0.42rem;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  justify-content: center;
}
.main_head li {
  float: left;
  width:1.1rem;
  line-height: .42rem;
  text-align:center;
}
</style>
 