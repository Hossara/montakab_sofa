<script setup lang="ts">
defineProps<{
  pattern: string,
  color: string
}>()
</script>

<template>
  <div class="sofa smallSofa">
    <img src="@/assets/objects/sofa_small.svg" alt="small_sofa">
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 1008 892" fill="none">
      <path d="M847.5 0.5L120.5 7C110.333 9 88.7 18.1 83.5 38.5C77 64 80.5 193 80.5 212C80.5 227.2 89.5 257 93 261C63.1667 293.667 3.09999 368.7 1.49999 407.5C-0.100011 446.3 13.5 476.333 20.5 486.5C29.6667 502.667 52.6 544.3 71 581.5C94 628 117.5 833 118 859C118.4 879.8 132.167 889 139 891H870.5C875.3 885 877.833 875.167 878.5 871C889.5 811 915.3 673 930.5 601C949.5 511 991.5 478 1000 451C1008.5 424 1011 378.5 996 354C984 334.4 924 276.833 895.5 250.5V53C895.5 13.8 863.5 1.66667 847.5 0.5Z" :fill="color" style="mix-blend-mode:color-burn"/>

      <defs>
        <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
          <use xlink:href="#image0_48_7" transform="matrix(0.00042337 0 0 0.00047788 0 -0.0643758)"/>
        </pattern>
      </defs>
    </svg>
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 1008 892" fill="none">
      <path d="M847.5 0.5L120.5 7C110.333 9 88.7 18.1 83.5 38.5C77 64 80.5 193 80.5 212C80.5 227.2 89.5 257 93 261C63.1667 293.667 3.09999 368.7 1.49999 407.5C-0.100011 446.3 13.5 476.333 20.5 486.5C29.6667 502.667 52.6 544.3 71 581.5C94 628 117.5 833 118 859C118.4 879.8 132.167 889 139 891H870.5C875.3 885 877.833 875.167 878.5 871C889.5 811 915.3 673 930.5 601C949.5 511 991.5 478 1000 451C1008.5 424 1011 378.5 996 354C984 334.4 924 276.833 895.5 250.5V53C895.5 13.8 863.5 1.66667 847.5 0.5Z" fill="url(#pattern0)" style="mix-blend-mode:color-burn"/>
      <defs>
        <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
          <use xlink:href="#image0_48_7" transform="matrix(0.00042337 0 0 0.00047788 0 -0.0643758)"/>
        </pattern>
        <image id="image0_48_7" width="2362" height="2362" :href="pattern"/>
      </defs>
    </svg>
  </div>
</template>

<style scoped lang="sass" src="@/assets/components/smallSofa.sass"></style>