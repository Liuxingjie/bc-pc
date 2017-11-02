<template>
            <div class="firstdetail">
                 <el-carousel>
                    <el-carousel-item v-for="item in msgs"  class="bgg">
                        <img :src="item.src" alt="">
                    </el-carousel-item>
                 </el-carousel>
                  <form action="http://www.baidu.com" name="myform" method="get">
                      <div class="formBox">
                        <div class="btnBox">
                            <button type="button" class="bgred bgfont20">免费设计</button>
                            <button type="button" class="bgfont20">预算报价</button>
                        </div>
                        <div class="inputBox">
                            <input type="text" required placeholder="您的称呼：" class="bgfont16"><br>
                            <input type="text" required placeholder="您的手机：" class="bgfont16"><br>
                        </div>
                        <select name="" id="" class="bgfont16">
                            <option value="">广东</option>
                        </select>
                        <select name="" id="" class="bgfont16">
                            <option value="">深圳</option>
                        </select>
                        <br>
                        <div class="free">
                            <button class="bgfont20 bgRed " type="submit">免费预约</button>
                        </div>
                        
                        <div class="shownumber">
                         已有<span class="bgred bgfont18">49327</span>业主申请
                        </div>
                     </div>
                 </form>     
            </div>
</template>
<script>
export default {
    props:[ 'msgs']
}
</script>
<style scoped>
  .firstdetail {
    width: 100%;
    height: 4.76rem;
    font-size:.1rem;
    position:relative;
  }
  .firstdetail img {
    width: 100%;
    cursor: pointer;
  }
  form {
    width: 2.88rem;
    height: 3.85rem;
    position: absolute;
    right: 0.5rem;
    top: 0.45rem;
    background: #fff;
    z-index:10;
  }
  .formBox {
    border: 1px solid #fedac1;
    width: 90%;
    height: 90%;
    margin: 5%;
  }
  .btnBox {
    width: 100%;
  }
  .btnBox button {
    width: 47%;
    border: none;
    background: none;
    padding: 0.2rem 0 0.1rem 0;
    font-size: 0.2rem;
    outline: none;
  }
  .inputBox {
    width: 100%;
  }
  .inputBox input {
    width: 100%;
    height: 0.3rem;
    /* padding:0.2rem 0; */
    margin: 0.1rem 0;
    border: none;
    border-bottom: 1px solid #7a7b78;
    outline: none;
  }
  select {
    width: 48%;
    border: none;
    outline: none;
    border-bottom: 1px solid #7a7b78;
    margin-top: 0.2rem;
    vertical-align: middle;
    color: #7a7b78;
  }
  .free {
    width: 100%;
    height: 0.9rem;
    border-bottom: 1px dashed red;
  }
  .free button {
    margin: 0.1rem 5%;
    width: 90%;
    border: none;
    outline: none;
    margin: 0.35rem 5%;
    padding: 0.02rem;
    color: white;
    border-radius: 0.05rem;
  }
  .shownumber {
    font-size: 0.14rem;
    text-align: center;
    vertical-align: center;
    padding-top: 0.15rem;
  }
</style>
