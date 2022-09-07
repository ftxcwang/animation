<template>
    <div class="svg-animate-demo">
        <div class="ball run_top_right"></div>
        <svg width='400' height='400'>
            <circle class="run_top_right" cx="42" cy="323" r="30" fill="greenyellow"></circle>
            <path d='M 42 323 C 209 345, 296 296, 348 221' stroke='red' stroke-width='10' fill='transparent'/>
        </svg>
    </div>
</template>
<script>
export default {
    name: 'SvgAnimateDemo',
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.svg-animate-demo{
    width: 400px;
    //定义动画的流程
    .run_top_right {
        display: block;
        animation: run-right-1 3s 0.4s 1 linear, run-right-2 3s 0.4s 1 cubic-bezier(.66, .1, .9, .41);
        // animation: run-right-right 3s 0.4s 1 linear, run-right-top 3s 0.4s 1 ease-out;
        animation-fill-mode: forwards;
    }
    //向上走的动画初始及结尾值
    @keyframes run-right-1 {
      0% {
        cx: 40px;
      }

      100% {
        cx: 348px;
      }
    }

    @keyframes run-right-2 {
      0% {
        cy: 323px;
      }
      100% {
        cy: 221px;
      }
    }
}
</style>
  