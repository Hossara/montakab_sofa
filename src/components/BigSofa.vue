<script setup lang="ts">
defineProps<{
  pattern: string,
  color: string
}>()
</script>

<template>
  <div class="sofa bigSofa">
    <img src="@/assets/objects/sofa_big.png" alt="bigSofa">
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 1747 961" fill="none">
      <path d="M53.5 334C36.5 357.5 9.5 396.5 1.9999 428C-3.65475 451.749 9.4999 492 17.9999 509.5C96.4999 642 86.4999 654.5 96.4999 689C103.931 714.637 121.667 831.333 126 888C129.2 926.8 133 946 145.5 950C172 969 1507 955 1555 954.5C1593.4 954.1 1604.33 938 1605 930C1622.5 865 1649 651 1681 585.5C1712.72 520.568 1715.5 529.5 1735.5 488.5C1755.5 447.5 1744 403.5 1728.5 375C1713 346.5 1619.5 268.5 1620 269C1620.4 269.4 1620.5 259.167 1620.5 254C1621.17 208.333 1622.5 105.2 1622.5 58C1622.5 10.8 1586.17 0.666674 1568 1.50001H182H131C110 6.50002 98 22.5 92 45C87.2 63 86.3333 105.5 86.5 124.5L89 220C88.2 239.6 97 265.167 101.5 275.5C93.9 283.1 66.6667 317 54 333"
            :fill="color" style="mix-blend-mode:color-burn"/>

      <defs>
        <pattern id="pattern1" patternContentUnits="objectBoundingBox" width="1" height="1">
          <use xlink:href="#image0_48_8" transform="matrix(0.00042337 0 0 0.00047788 0 -0.0643758)"/>
        </pattern>
      </defs>
    </svg>
    <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"  viewBox="0 0 1747 961" fill="none">
      <path d="M53.5 334C36.5 357.5 9.5 396.5 1.9999 428C-3.65475 451.749 9.4999 492 17.9999 509.5C96.4999 642 86.4999 654.5 96.4999 689C103.931 714.637 121.667 831.333 126 888C129.2 926.8 133 946 145.5 950C172 969 1507 955 1555 954.5C1593.4 954.1 1604.33 938 1605 930C1622.5 865 1649 651 1681 585.5C1712.72 520.568 1715.5 529.5 1735.5 488.5C1755.5 447.5 1744 403.5 1728.5 375C1713 346.5 1619.5 268.5 1620 269C1620.4 269.4 1620.5 259.167 1620.5 254C1621.17 208.333 1622.5 105.2 1622.5 58C1622.5 10.8 1586.17 0.666674 1568 1.50001H182H131C110 6.50002 98 22.5 92 45C87.2 63 86.3333 105.5 86.5 124.5L89 220C88.2 239.6 97 265.167 101.5 275.5C93.9 283.1 66.6667 317 54 333"
            fill="url(#pattern1)" style="mix-blend-mode:color-burn"/>
      <defs>
        <pattern id="pattern1" patternContentUnits="objectBoundingBox" width="1" height="1">
          <use xlink:href="#image0_48_8" transform="matrix(0.00042337 0 0 0.00047788 0 -0.0643758)"/>
        </pattern>
        <image id="image0_48_8" width="2362" height="2362" :href="pattern"/>
      </defs>
    </svg>
  </div>
</template>

<style scoped lang="sass" src="@/assets/components/bigSofa.sass"></style>