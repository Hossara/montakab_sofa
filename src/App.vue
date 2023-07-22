<script setup lang="ts">
import {ref} from "vue"
import SmallSofa from "@/components/SmallSofa.vue"
import BigSofa from "@/components/BigSofa.vue"

import p1 from "@/assets/patterns/1.png"
import p2 from "@/assets/patterns/2.png"
import ControlPanel from "@/components/ControlPanel.vue"
import CurtainLeft from "@/components/curtainLeft.vue";
import CurtainRight from "@/components/curtainRight.vue";


const patterns = ref([
    p1, p2
])

const active_sofa1_pattern = ref(patterns.value[0])
const active_sofa1_color = ref("#ffffff")

const active_sofa2_pattern = ref(patterns.value[0])
const active_sofa2_color = ref("#ffffff")

const active_curtain_pattern = ref(patterns.value[0])
const active_curtain_color = ref("#ffffff")


const changeColor = (sofa: number, color: string) => {
  switch (sofa) {
    case 1:
      active_sofa1_color.value = color
      break
    case 2:
      active_sofa2_color.value = color
      break
    case 3:
      active_curtain_color.value = color
      break
  }
}

const changePattern = (sofa: number, index: number) => {
  switch (sofa) {
    case 1:
      active_sofa1_pattern.value = patterns.value[index]
      break
    case 2:
      active_sofa2_pattern.value = patterns.value[index]
      break
    case 3:
      active_curtain_pattern.value = patterns.value[index]
      break
  }
}
</script>

<template>
  <main>
    <ControlPanel :patterns="patterns" @changeColor="changeColor" @changePattern="changePattern"/>
    <CurtainLeft :color="active_curtain_color" :pattern="active_curtain_pattern"/>
    <CurtainRight :color="active_curtain_color" :pattern="active_curtain_pattern"/>
    <SmallSofa :pattern="active_sofa1_pattern" :color="active_sofa1_color"/>
    <BigSofa :pattern="active_sofa2_pattern" :color="active_sofa2_color"/>
  </main>
</template>

<style src="@/assets/main.sass" lang="sass"></style>