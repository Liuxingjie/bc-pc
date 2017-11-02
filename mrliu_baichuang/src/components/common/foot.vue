<template>
      <div id="foot">
        <div class="box">
            <div class="headBox">
              <ul>
                <li class="logo fl">
                  <img src="../../../static/images/logofoot.png" >
                </li>
                <li class="details1 fl">
                  <ul >
                    <li class="fl li1 borderLeft">
                        <ul>
                          <li class="bgfont14 bgwhite">了解百创</li>
                          <li>首页</li>
                          <li>公司简介</li>
                          <li>企业优势</li>
                          <li>特色服务</li>
                        </ul>
                    </li>
                    <li class="fl li1">
                        <ul>
                          <li class="bgfont14 bgwhite">产品介绍</li>
                          <li>新房装修</li>
                          <li>旧房改造</li>
                          <li>软装配置</li>
                        </ul>
                    </li>
                    <li class="fl li1 borderRight">
                      <ul>
                        <li class="bgfont14 bgwhite">品台服务</li>
                        <li>设计与报价</li>
                        <li>效果图</li>
                        <li>装修攻略</li>
                      </ul>
                    </li>
                  </ul>
                </li>
                <li class="details2 fl">
                  <h3>联系我们</h3>
                  <span>400-800-6266</span>
                  <button>在线客服</button>
                </li>
              </ul>
            </div>
            <div class="footBox">
                <ul>
                  <li>友情链接</li>
                  <li><a href="#">智能家</a></li>
                  <li><a href="#">临析房产网</a></li>
                  <li><a href="#">工长俱乐部</a></li>
                  <li><a href="#">东莞装修网</a></li>
                  <li><a href="#">武汉一号家居网</a></li>
                  <li><a href="#">天津办公家具</a></li>
                  <li><a href="#">创意家居</a></li>
                  <li><a href="#">家具智能化</a></li>
                  <li><a href="#">成都装修公司</a></li>
                  <li><a href="#">济南装修网</a></li>
                  <li><a href="#">深圳办公家具</a></li>
                </ul>
            </div>
            <div class="certificate">
                <h4>@2015-2020 深圳市百创网络科技有限公司，并保留所有权利&nbsp;ICP备案证书号:粤ICP备15062620号</h4>
            </div>
        </div>
      </div>
</template>
<script>
export default {};
</script>
<style scoped>
 #foot{
   width:100%;
   height:2.72rem;
   background:#393939;
   color: white;
   font-size: .12rem;
  }
 #foot .box{
   width:100%;
   height: 100%;
   position: relative;
  }
 #foot .box .headBox{
   width:9.07rem;
   height: 2rem;
   padding-top:.34rem;
   border-bottom:1px dashed gray;
   margin:0 auto;
  }
 #foot .box .logo{
   width:2.62rem;
   height: 2rem;
  }
  .borderRight{
    border-right: 1px dashed gray;
  }
 #foot .box .details1{
   width:3.66rem;
   height: 100%;
  }
 #foot .box .details1 .li1{
    text-align:center;
    width:33.3%; 
    height: 100%;
    font-size: .12rem;
    color: #908f8f;
  }

 #foot .box .details1 .li1 ul li{
   padding-bottom:.16rem;
  }
#foot .box .details2{
    width:2.54rem;
    height: 100%;
    padding-left:.44rem;
 }
#foot .box .footBox{
  position: relative;
  left: -2.3rem;;
  width:100%;
  height:.46rem;

 }
 #foot .box .footBox ul{
   width:100%;
   height: 100%;
 }
 #foot .box .footBox li{
   font-size: .12rem;
   float: left;
   padding-right:.1rem;
   line-height: .46rem;
 }
  #foot .box .footBox li a{
    color: #908f8f;
  }
 #foot .box .certificate{
   width:100%;
   height: .26rem;
   text-align:center;
   background:#1c1c1c;
   line-height: .26rem;
   font-size: .14rem;
   color: #908f8f;
 }

</style>
