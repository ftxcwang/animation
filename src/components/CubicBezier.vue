<template>
    <div class="cubic-bezier">
        <svg class="g-svg" width="400" height="160" xmlns="http://www.w3.org/2000/svg">
            <path d="M 10 80 C 80 10, 130 10, 190 80 S 300 150, 360 80" stroke="black" fill="transparent"/>
        </svg>
        <div class="g-wrap">
            <div class="ball"></div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'CubicBezier',
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.cubic-bezier{
    position: relative;
    .g-svg {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
    .g-wrap {
        position: relative;
        width: 400px;
        height: 160px;
        margin: auto;
        // outline: 1px solid #000;
        .ball {
            position: aboslute;
            width: 40px;
            height: 40px;
            clip-path: polygon(0 0, 100% 50%, 0 100%);
            offset-path: path('M 10 80 C 80 10, 130 10, 190 80 S 300 150, 360 80');
            offset-anchor: 0 100%;
            background: linear-gradient(#fc0, #f0c);
            animation: move 3000ms infinite alternate linear;
        }
    }
    @keyframes move {
        0% {
            offset-distance: 0%;
        }
        100% {
            offset-distance: 100%;
        }
    }
}
</style>
  