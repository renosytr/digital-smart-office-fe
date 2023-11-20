<template>
  <div>
    <img :src="props.image"/>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  image: string;
}>();
</script>
