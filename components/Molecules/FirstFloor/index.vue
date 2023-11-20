<template>
  <AtomsFloor
    image="/images/floors/desk-first-32.png"
    canvasWidth="2574"
    canvasHeight="1209"
    :grid="grid"
  >
    <AtomsFloorLibraryRoom
      :data-user-library="dataUserLibrary"
    ></AtomsFloorLibraryRoom>
  </AtomsFloor>
</template>
<script setup lang="ts">
import { ref } from "vue";
import type { Ref } from "vue";
import { grid } from "@/assets/grid-room/first-floor-32";

const dataUserLibrary: any[] = [
  {
    image: null,
    name: null,
  },
  {
    image: null,
    name: null,
  },
  {
    image: null,
    name: null,
  },
  {
    image: null,
    name: null,
  },
  {
    image: null,
    name: null,
  },
  {
    image: null,
    name: null,
  },
];
</script>
