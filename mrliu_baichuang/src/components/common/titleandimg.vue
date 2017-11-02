<template>
    <div>
            <div class="textcenter  setmeal">
                <h3 class="bgred bgfont24">{{titleandimg.title}}</h3>
                <img :src="titleandimg.src">
            </div>
    </div>
</template>
<script>
export default {
   props:['titleandimg']
}
</script>
<style scoped>
.setmeal {
    width: 100%;
    padding-bottom: 0.31rem;
  }
  .setmeal h3 {
    line-height: 1.46rem;
  }
</style>
