<template>
  <div class="w-max relative">
    <slot></slot>
    <canvas
      :width="canvasWidth"
      :height="canvasHeight"
      class="absolute z-10"
    ></canvas>
    <img :src="props.image" />
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  image: string;
  grid: number[][];
  canvasWidth: string;
  canvasHeight: string;
}>();
</script>
