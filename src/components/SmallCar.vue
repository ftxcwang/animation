<template>
    <div className='car-wrapper'>
            <div className='demo-wrapper'>
              <div className='car'>
                  <div className='car-body'>
                      <div className='adorn1'></div>
                      <div className='adorn2'></div>
                      <div className='adorn3'></div>
                  </div>
                  <div className='tube'></div>
                  <div className='wheel left-wheel'>
                      <div className='line1'></div>
                      <div className='line2'></div>
                      <div className='line3'></div>
                      <div className='line4'></div>
                      <div className='line5'></div>
                  </div>
                  <div className='wheel right-wheel'>
                      <div className='line1'></div>
                      <div className='line2'></div>
                      <div className='line3'></div>
                      <div className='line4'></div>
                      <div className='line5'></div>
                  </div>
                  <div className='car-head'>
                      <div className='left-wind'></div>
                      <div className='right-wind'></div>
                  </div>
                  <div className='ball1'></div>
                  <div className='ball2'></div>
                  <div className='ball3'></div>
                  <div className='weiqi1'></div>
                  <div className='weiqi2'></div>
              </div>
              <div className='street-wrap'>
                  <div className='street street1'>
                      <div className='stone'>
                          <div className='stone1'></div>
                          <div className='stone2'></div>
                          <div className='stone3'></div>
                          <div className='stone4'></div>
                      </div>
                  </div>
                  <div className='street street2'>
                      <div className='stone'>
                          <div className='stone1'></div>
                          <div className='stone2'></div>
                          <div className='stone3'></div>
                          <div className='stone4'></div>
                      </div>
                  </div>
              </div>
              <div className='cloud-wrap'>
                    <div className='cloud1'></div>
                    <div className='cloud2'></div>
                    <div className='cloud3'></div>
                    <div className='cloud4'></div>
              </div>
            </div>
      </div>
</template>
<script>
export default {
    name: 'SmallCar'
}
</script>
<style scoped lang="less">
.car-wrapper{
  // background: #c5f6f6;
  .demo-wrapper{
    padding: 0px;
    position: relative;
    top: 317px;
    margin-left: 50px;
    .car{
      width:  400px;
      margin:  0  auto;
      .car-body{
        width:  238px;
        height:  54px;
        background:  #f06043;
        border-radius:  30px;
        margin:  0  auto;
        position:  relative;
        animation:  car  0.5s  infinite  linear;
        z-index:  2;
        .adorn1{
          width:  17px;
          height:  6px;
          background:  #d24629;
          border-radius:  50%;
          transform:  rotate(-60deg);
          position:  absolute;
          top:  12px;
          left:  -1px;
        }
        .adorn2{
          width:  25px;
          height:  5px;
          background:  #fff;
          position:  absolute;
          top:  20px;
          left:  86px;
          border-radius:  10px;
        }
        .adorn3{
          width:  17px;
          height:  6px;
          background:  #fff;
          border-radius:  50%;
          transform:  rotate(-123deg);
          position:  absolute;
          top:  12px;
          left:  224px;
        }
      }
      .tube{
        width:  10px;
        height:  6px;
        background:  #333;
        position:  relative;
        top:  -13px;
        left:  81px;
        z-index:  1;
        border-radius:  30%  0  0  30%;        
      }
      .wheel{
        height:  35px;
        border:  5px  solid  #333;
        border-radius:  50%;
        background:  #fff;
        position:  relative;
        z-index:  10;
        &:after{
          content:  '';
          position:  absolute;
          top:  15px;
          left:  15px;
          width:  6px;
          height:  6px;
          border-radius:  50%;
          background-color:  #333;
        }
        &.left-wheel{
          left:  106px;
          animation:  leftwheel  0.4s  infinite  linear;
        }
        &.right-wheel{
          left:  246px;
          animation:  rightwheel  0.4s  infinite  linear;
        }
        div{
          width:  4px;
          height:  10px;
          background:  #353535;
          position:  absolute;
          &.line1{
            transform:  rotate(-54deg);
            top:  6px;
            left:  8px;
          }
          &.line2{
            transform:  rotate(-125deg);
            left:  8px;
            top:  19px;
          }
          &.line3{
            transform:  rotate(-202deg);
            left:  20px;
            top:  22px;
          }
          &.line4{
            transform:  rotate(-270deg);
            left:  26px;
            top:  13px;
          }
          &.line5{
            transform: rotate(22deg);
            left: 20px;
            top: 4px;
          }
        }
      }
      .car-head{
        width: 163px;
        height: 38px;
        background: #333;
        position: relative;
        -webkit-clip-path: polygon(5% 0,80% 0, 100% 100%, 0 100%);
        animation: window 0.5s infinite linear;
        .left-wind{
          width: 50px;
          height: 26px;
          background: -webkit-linear-gradient(bottom, #88d6e7, #e4ffff);
          position: absolute;
          left: 10px;
          top: 8px;
          -webkit-clip-path: polygon(10% 0, 100% 0, 100% 100%, 0 100%);
        }
        .right-wind{
          width: 78px;
          height: 26px;
          background: -webkit-linear-gradient(bottom, #88d6e7, #e4ffff);
          position: absolute;
          left: 69px;
          top: 8px;
          -webkit-clip-path: polygon(0% 0, 71% 0, 100% 100%, 0 100%);
        }
      }
      .ball1{
        width: 20px;
        height: 25px;
        background: #d72535;
        border-radius: 50%;
        position: relative;
        animation: ball1 2s infinite linear;
        animation-direction:alternate;
        &:before{
          content: '';
          position: absolute;
          top: 4px;
          left: 14px;
          width: 3px;
          height: 5px;
          background-color: #fff;
          border-radius: 50%;
        }
        &:after{
          content: '';
          position: absolute;
          top: 49px;
          left: -15px;
          width: 50px;
          height: 1px;
          background-color: rgba(0,0,0,0.5);
          transform: rotate(-90deg);
        }
      }
      .ball2{
        width: 20px;
        height: 25px;
        background: #fde000;
        border-radius: 50%;
        position: relative;
        animation: ball2 2s infinite linear;
        animation-direction:alternate;
        &:before{
          content: '';
          position: absolute;
          top: 4px;
          left: 14px;
          width: 3px;
          height: 5px;
          background-color: #fff;
          border-radius: 50%;
        }
        &:after{
          content: '';
          position: absolute;
          top: 60px;
          left: -24px;
          width: 71px;
          height: 1px;
          background-color: rgba(0,0,0,0.5);
          transform: rotate(-90deg);
        }
      }
      .ball3{
        width: 20px;
        height: 25px;
        background: #0287ca;
        border-radius: 50%;
        position: relative;
        animation: ball3 2s infinite linear;
        animation-direction:alternate;
        &:before{
          content: '';
          position: absolute;
          top: 4px;
          left: 14px;
          width: 3px;
          height: 5px;
          background-color: #fff;
          border-radius: 50%;
        }
        &:after{
          content: '';
          position: absolute;
          top: 71px;
          left: -38px;
          width: 95px;
          height: 1px;
          background-color: rgba(0, 0, 0, 0.5);
          transform: rotate(-90deg);
        }
      }
      .weiqi1{
        border-radius: 50%;
        background: #999;
        position: absolute;
        z-index: 0;
        animation: weiqi 1s infinite linear;
      }
      .weiqi2{
        border-radius: 50%;
        background: #999;
        position: absolute;
        animation: weiqi 1s infinite linear;
        animation-delay:0.5s;
        z-index: 0;
      }
    }
    .street-wrap{
      position: absolute;
      overflow: hidden;
      width: 100%;
      height: 200px;
      top: 80px;
      .street{
        width: 100%;
        height: 200px;
        background: #88d6e7;
        position: relative;
        .stone{
          position: relative;
          .stone1{
            width: 40px;
            height: 15px;
            background: #36a3b9;
            border-radius: 20px 20px 0px 0px;
            position: relative;
            top: 8px;
            left: 15%;
          }
          .stone2{
            width: 20px;
            height: 10px;
            background: #36a3b9;
            border-radius: 10px 10px 0px 0px;
            position: relative;
            top: 40px;
            left: 35%;
          }
          .stone3{
            width: 30px;
            height: 12px;
            background: #36a3b9;
            border-radius: 13px 13px 0px 0px;
            position: relative;
            top: 9px;
            left: 50%;
          }
          .stone4{
            width: 35px;
            height: 14px;
            background: #36a3b9;
            border-radius: 13px 13px 0px 0px;
            position: relative;
            top: -18px;
            left: 78%;
          }
        }
        &.street1{
          animation: street1 4s infinite linear;
        }
        &.street2{
          top: -200px;
          animation: street2 4s infinite linear;
        }
      }
    }
    .cloud-wrap{
      position: absolute;
      top: -320px;
      width: 100%;
      overflow: hidden;
      background: #c5f6f6;
      z-index: -1;
      .cloud1{
        width: 250px;
        height:150px;
        background: url('../../img/cloud1.png') no-repeat;
        background-size: contain;
        position: relative;
        animation: cloud1 18s infinite linear;
      }
      .cloud2{
        width: 250px;
        height:150px;
        background: url('../../img/cloud2.png') no-repeat;
        position: relative;
        background-size: contain;
        animation: cloud2 18s infinite linear;
      }
      .cloud3{
        width: 250px;
        height:150px;
        background: url('../../img/cloud3.png') no-repeat;
        position: relative;
        background-size: contain;
        top: -240px;
        animation: cloud3 18s infinite linear;
      }
      .cloud4{
        width: 250px;
        height:150px;
        background: url('../../img/cloud4.png') no-repeat;
        position: relative;
        background-size: contain;
        top: -480px;
        animation: cloud4 18s infinite linear;
      }
    }
  }
  .introduce-wrapper{
    position: relative;
    top: 300px;
  }
}
@keyframes window{
  0%{
    top: -182px;
    left: 104px;
  }
  100%{
    top: -180px;
    left: 106px;
  }
}
@keyframes car{
  0%{
    top: 0px;
    left: 0px;
  }
  100%{
    top: 2px;
    left: 2px;
  }
}
@keyframes leftwheel{
  0%{ 
    top: -23px;
    transform:rotate(0deg);
    width: 35px;
  }
  100%{ 
    top: -25px;
    transform:rotate(360deg);
    width: 38px;
  }
}
@keyframes rightwheel{
  0%{ 
    top: -68px;
    transform:rotate(0deg);
    width: 35px;
  }
  100%{ 
    top: -70px;
    transform:rotate(360deg);
    width: 38px;
  }
}
@keyframes ball1{
  0%{
    transform: rotate(-45deg);
    top: -239px;
    left: 52px;
  }
  100%{
    transform: rotate(-30deg);  
    top: -251px;
    left: 65px;
  }
}
@keyframes ball2{
  0%{
    transform: rotate(-20deg);
    top: -297px;
    left: 67px;
  }
  100%{
    transform: rotate(-45deg);  
    top: -279px;
    left: 36px;
  }
}
@keyframes ball3{
  0%{
    transform: rotate(-30deg);
    top: -337px;
    left: 44px;
  }
  100%{
    transform: rotate(-60deg);  
    top: -298px;
    left: 5px;
  }
}
@keyframes street1{
  0%{left: 0}
  100%{left: -100%}
}
@keyframes street2{
  0%{left: 100%}
  100%{left: 0%}
}
@keyframes cloud1{
  0%{left: 10%}
  15%{left:-20%}
  15.05%{left: 180%}
  100%{left: 10%}
}
@keyframes cloud2{
  0%{left: 75%; top: -160px;}
  47.5%{left:-20%;top:-140px;}
  47.55%{left: 180%}
  100%{left: 75%;top:-160px}
}
@keyframes cloud3{
  0%{left: 125%}
  72.5%{left:-20%}
  72.55%{left: 180%}
  100%{left: 125%}
}
@keyframes cloud4{
  0%{left: 170%}
  95%{left:-20%}
  95.05%{left: 180%}
  100%{left: 170%}
}
@keyframes weiqi{
  0%{
    width: 5px;
    height: 5px;
    opacity: 1;
    top: 42px;
    left: 300px;
  }
  100%{
    opacity: 0;
    width: 20px;
    height: 20px;
    top: 15px;
    left: 270px;
  }
}
</style>