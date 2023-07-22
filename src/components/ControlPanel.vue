<script setup lang="ts">
import {ref} from "vue"

defineProps<{
  patterns: string[]
}>()

const emit = defineEmits()

const sofa1_color = ref("#ffffff")
const sofa2_color = ref("#ffffff")
const curtain_color = ref("#ffffff")

const sofa1_pattern = ref(0)
const sofa2_pattern = ref(0)
const curtain_pattern = ref(0)

const changeColor = (sofa: number, data: any) => {
  emit("changeColor", sofa, data)
}

const changePattern = (sofa: number, data: number) => {
  emit("changePattern", sofa, data)
}
</script>

<template>
  <div class="controlPanel">
    <div class="item">
      <h5>Sofa 1</h5>
      <label>
        Color
        <input type="color" v-model="sofa1_color" @change="changeColor(1, sofa1_color)">
      </label>

      <label>
        Pattern
        <select v-model="sofa1_pattern" @change="changePattern(1, sofa1_pattern)">
          <option v-for="(pattern, index) in patterns" :key="pattern" :value="index">pattern {{index}}</option>
        </select>
      </label>
    </div>
    <div class="item">
      <h5>Sofa 2</h5>
      <label>
        Color
        <input type="color" v-model="sofa2_color" @change="changeColor(2, sofa2_color)">
      </label>

      <label>
        Pattern
        <select v-model="sofa2_pattern" @change="changePattern(2, sofa2_pattern)">
          <option v-for="(pattern, index) in patterns" :key="pattern" :value="index">pattern {{index}}</option>
        </select>
      </label>
    </div>
    <div class="item">
      <h5>Curtain</h5>
      <label>
        Color
        <input type="color" v-model="curtain_color" @change="changeColor(3, curtain_color)">
      </label>

      <label>
        Pattern
        <select v-model="curtain_pattern" @change="changePattern(3, curtain_pattern)">
          <option v-for="(pattern, index) in patterns" :key="pattern" :value="index">pattern {{index}}</option>
        </select>
      </label>
    </div>
  </div>
</template>

<style scoped lang="sass" src="@/assets/components/controlPanel.sass"></style>