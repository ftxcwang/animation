<template>
  <div class="about">
      <!-- <div>
        <CubicBezier />
        <SvgAnimate />
        <SvgAnimateDemo />
        <SvgAnimateOnly />
        <LightHouse1 />
      </div>
      <LightHouse /> -->
      <CableCar />
  </div>
</template>
<script>
import CubicBezier from '@/components/CubicBezier.vue'
import SvgAnimate from '@/components/SvgAnimate.vue'
import SvgAnimateDemo from '@/components/SvgAnimateDemo.vue'
import SvgAnimateOnly from '@/components/SvgAnimateOnly.vue'
import LightHouse from '@/components/LightHouse.vue'
import LightHouse1 from '@/components/LightHouse1.vue'
import CableCar from '@/components/CableCar.vue'

export default {
    name: 'About',
    components: {
      CubicBezier,
      SvgAnimate,
      SvgAnimateDemo,
      SvgAnimateOnly,
      LightHouse,
      LightHouse1,
      CableCar,
  }
}
</script>
<style lang="less">
</style>