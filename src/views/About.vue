<template>
  <div class="about">
      <div>
        <CubicBezier />
        <SvgAnimate />
        <SvgAnimateDemo />
        <SvgAnimateOnly />
      </div>
      <LightHouse />
  </div>
</template>
<script>
import CubicBezier from '@/components/CubicBezier.vue'
import SvgAnimate from '@/components/SvgAnimate.vue'
import SvgAnimateDemo from '@/components/SvgAnimateDemo.vue'
import SvgAnimateOnly from '@/components/SvgAnimateOnly.vue'
import LightHouse from '@/components/LightHouse.vue'

export default {
    name: 'About',
    components: {
      CubicBezier,
      SvgAnimate,
      SvgAnimateDemo,
      SvgAnimateOnly,
      LightHouse,
  }
}
</script>
<style lang="less">
  .about{
    background: #ddd;
    display: flex;
  }
</style>