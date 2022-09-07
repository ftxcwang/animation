<template>
  <div class="about">
      <CubicBezier />
      <SvgAnimate />
      <SvgAnimateDemo />
  </div>
</template>
<script>
import CubicBezier from '@/components/CubicBezier.vue'
import SvgAnimate from '@/components/SvgAnimate.vue'
import SvgAnimateDemo from '@/components/SvgAnimateDemo.vue'
export default {
    name: 'About',
    components: {
      CubicBezier,
      SvgAnimate,
      SvgAnimateDemo,
  }
}
</script>

<style lang="less">
</style>