<template>
    <div id="overAll">
        <heads ></heads>
        <firstdetail :msgs='mesg'></firstdetail>
        <foots></foots>
    </div>
</template>
<script>
import heads from "@/components/common/head"
import foots from "@/components/common/foot"
import firstdetail from "@/components/common/firstdetail"
export default {
    data(){
        return{
            mesg:[{src:'../../static/images/zhengtitaozhuang1_02.png'}]
        }
    },
    components:{ heads,foots ,firstdetail}
}
</script>
<style scoped>
    .bgred1{
        color:#7e7e7e;
    }
    .bgred2{
        color:red;
    }
</style>
