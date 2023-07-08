<script setup lang="ts">
import {ref} from "vue";

defineProps<{
  patterns: string[]
}>()

const emit = defineEmits()

const sofa1_color = ref("#ffffff")
const sofa2_color = ref("#ffffff")
const sofa1_pattern = ref(0)
const sofa2_pattern = ref(0)

const changeSofaColor = (sofa: number, data: any) => {
  emit("changeSofaColor", sofa, data)
}

const changeSofaPattern = (sofa: number, data: number) => {
  emit("changeSofaPattern", sofa, data)
}
</script>

<template>
  <div class="controlPanel">
    <div class="item">
      <h5>Sofa 1</h5>
      <label>
        Color
        <input type="color" v-model="sofa1_color" @change="changeSofaColor(1, sofa1_color)">
      </label>

      <label>
        Pattern
        <select v-model="sofa1_pattern" @change="changeSofaPattern(1, sofa1_pattern)">
          <option v-for="(pattern, index) in patterns" :key="pattern" :value="index">pattern {{index}}</option>
        </select>
      </label>
    </div>
    <div class="item">
      <h5>Sofa 2</h5>
      <label>
        Color
        <input type="color" v-model="sofa2_color" @change="changeSofaColor(2, sofa2_color)">
      </label>

      <label>
        Pattern
        <select v-model="sofa2_pattern" @change="changeSofaPattern(2, sofa2_pattern)">
          <option v-for="(pattern, index) in patterns" :key="pattern" :value="index">pattern {{index}}</option>
        </select>
      </label>
    </div>
  </div>
</template>

<style scoped lang="sass" src="@/assets/components/controlPanel.sass"></style>