<template>
  <div id="home">
      <heads :istrue='istrue' :red='red'></heads>
         <div class="main_content">
             <firstdetail :msgs='msgs'></firstdetail>
            <titleandimg :titleandimg="titleandimg"></titleandimg>
            <div>
                <img src="../../static/images/home3.png" >
            </div>
            <div class="swipeBox">
                <div class="titleBox">
                         <h3 class="bgred bgfont24">九大特色工艺</h3><br>
                        <p>16年家装工艺保障，自信源于实力</p>
                </div>
               
                <div class="swipe">
                        <div class="maxWidth"  >
                            <ul id="maxWidthul">
                                <li v-for="item in teseImg">
                                    <img :src="item.src" >
                                    <p>{{item.title}}</p>
                                </li>
                             </ul>
                             <span class="positionleft" @click='translateLeft'> <</span>
                             <span class="positionright" @click='translateRight'> ></span>
                        </div>
                </div>
            </div>
            <div class="tiyan">
                <div>
                    <h3 class="bgred bgfont24">3D体验</h3>
                    <ul>
                        <li class="bgred">时尚北欧</li>
                        <li>原木之家</li>
                        <li>现代英伦风</li>
                        <li>田园风格</li>
                        <li>中式风格</li>
                    </ul>
                </div>
            </div>
            <div>
                <img src="../../static/images/home4.png">
            </div>
            <div class="tiyan">
                <div>
                    <h3 class="bgred bgfont24"> 工地直播</h3>
                    <ul>
                        <li class="bgred">领丽花园</li>
                        <li>尚峰</li>
                    </ul>
                </div>
            </div>
            <div class="zhibo">
                <div class="zhiboBox">
                    <img src="../../static/images/home5.png">
                    <div class="zhiboTitle">
                        <ul>
                            <li><h3 class="bgfont16 bgclassfb5919">领航城领丽花园C-602</h3></li>
                            <li>
                                <ul class="ul1">
                                    <li>南山区</li>
                                    <li>二居室</li>
                                    <li>75m<sup>2</sup></li>
                                    <li>35天</li>
                                    <li>999套餐</li>
                                </ul>
                            </li>
                            <li>

                            </li>
                            <li>
                                <ul class="clear ul2">
                                    <li class="bgfb5919_7">开工大吉</li>
                                    <li class="bgfb5919_7">水电工程</li>
                                    <li class="bgfb5919_7">瓦工工程</li>
                                    <li class="bgclassfb5919">水工工程</li>
                                    <li class="bggray">油漆工程</li>
                                    <li class="bggray">安装阶段</li>
                                </ul>
                            </li>
                        </ul>
                        <button class="btncanguan">预约参观</button>
                    </div>
               </div>
            </div>
            <div class="tiyan">
                <div>
                    <h3 class="bgred bgfont24"> 设计师团队</h3>
                    <ul>
                        <li  class="bgred">更多>>></li>
                    </ul>
                </div>
            </div>
            <div class="designteam">
                <div class="designBox">
                    <ul class="ul1">
                        <li class="li1">
                          <button>找他设计</button>
                          <img src="../../static/images/liuxingjie_03.png" >
                          <div class="coverBox">
                              <span class="bgfont16">何春林&nbsp;&nbsp;&nbsp;资深设计师</span>
                              <p>设计经验：7年  &nbsp;&nbsp;&nbsp;作品：130个&nbsp;&nbsp;&nbsp;&nbsp;人气：2330</p>
                          </div>
                        </li>
                        <li class="li2">
                            <img src="../../static/images/lunbotu1_03.png">
                            <div class="positionAimgs positionBs">
                            </div>
                        </li>
                        <li class="li3">
                            <ul class="ul2">
                                <li tabindex="1"><img src="../../static/images/lunbotu1_13.png" alt=""></li>
                                <li  tabindex="1"><img src="../../static/images/lunbotu1_09.png" alt=""></li>
                                <li  tabindex="1"><img src="../../static/images/smallPic_09.png" alt=""></li>
                            </ul>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="tiyan">
                <div>
                    <h3 class="bgred bgfont24"> 装修攻略</h3>
                    <ul>
                      <li class="bgred">装修日记</li>
                      <li>装修风水</li>
                      <li>建材手册</li>
                      <li>装修知识</li>
                      <li>更多>>> </li>
                    </ul>
                </div>
            </div>
            <div class="fitment">
                <ul>
                    <li v-for="item in fitment">
                        <img :src="item.src">
                        <h3 class="bgfont16">{{item.title}}</h3>
                        <p>{{item.explain}}</p>
                    </li>
                </ul>
            </div>
            <div class="tiyan">
                <div>
                    <h3 class="bgred bgfont24"> 公司动态</h3>
                </div>
            </div>
            <div>
                <img src="../../static/images/gongsi_14.png" alt="">
            </div>
            <foots></foots>
      </div>
  </div>
</template>
<script>
import heads from "@/components/common/head"
import foots from "@/components/common/foot"
import firstdetail from "@/components/common/firstdetail"
import titleandimg from "@/components/common/titleandimg"
export default {
    data(){
        return{
            fitment:[
                { src:'../../static/images/home7.png',title:'家居生活中7个健康细节',explain:'家具生活中难免会忽略各种健康细节，下面就让百创为大家整理一下，家居生活中容易被忽...' },
                {src:'../../static/images/home8.png',title:'一枚伪文艺菇凉的单身公寓',explain:'留白是种艺术，收纳是门学问!细数你在客厅中缺一不可的物件，然后把多余的都...'},
                {src:'../../static/images/home9.png',title:'欧式风格简约装修',explain:'50平米的空间极致的欧式装修设计，回归自然的洁净，原木色的木板更加...'}
            ],
            titleandimg:{ src:"../../static/images/home2.png ",title:'百创套餐'},
            msgs:[
                 {src:'../../static/images/home1.jpg'},
                {src:'../../static/images/taocan_02.png'}
                ],
            teseImg:[
                {src:'../../static/images/jiaju1.jpg',title:'形象工艺保护'},
                {src:'../../static/images/jiaju2.jpg',title:'个性家居'},
                {src:'../../static/images/jiaju3.jpg',title:'命名环境'},
                {src:'../../static/images/jiaju4.jpg',title:'门梁工艺'}
            ],
            shejishi:[
                {src:''}
            ],
            istrue:true
        }
    },
  components: { heads ,foots,firstdetail,titleandimg},
  methods:{
      translateLeft(){
          var ul =  document.getElementById('maxWidthul')
            ul.style.left = ul.style.left.replace('rem','') - 2.9 + 'rem'
      }
      , translateRight(){
            var ul =  document.getElementById('maxWidthul')
         if(ul.style.left >='0rem'){
             ul.style.left =-11.6+'rem' 
         }
         else{
                 ul.style.left = ul.style.left.replace('rem','') - 0 + 2.9 + 'rem';
         }
    
      }
  }
};
</script>
<style scoped>
 @import url(../style/home.css);
.bgg{
    width:100%;
    height: 4.76rem;
}
.designBox .ul2 li:focus{
    border:2px solid lightblue;
}
</style>    
