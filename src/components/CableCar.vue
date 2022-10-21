<template>
    <div class="container">
        <div class="cable-car">
            <div class="line"></div>
            <!-- <div class="car1"></div> -->
            <div class="car2"></div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'CableCar',
}
</script>
<style scoped lang="less">
.container{
    width: 300px;
    height: 600px;
    background: #FFFFFF;
    .cable-car{
        position: relative;
        .line{
            height: 3px;
            background: #e08811;
            width: 300px;
            transform: rotate(-15deg);
            position: absolute;
            top: 100px;
        }
        .car1{
            width: 40px;
            height: 40px;
            background: #00F;
            // transform: rotate(15deg);
            position: absolute;
            top: 140px;
            left: 10px;
        }
        .car2{
            width: 40px;
            height: 40px;
            background: #00F;
            transform: rotate(10deg);
            position: absolute;
            top: 140px;
            left: 10px;
            animation: move 5s 0s infinite;
        }
        @keyframes move {
            from, to{
                transform: rotate(10deg);
            }
            50% {
                transform: translateX(260px) translateY(-70px) translateZ(0) rotate(10deg);
            }
        }
    }
}
</style>
  