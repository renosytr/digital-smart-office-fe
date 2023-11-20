<template>
  <AtomsFloorMainCanvas
    image="/images/floors/desk-first-32.png"
    canvas-width="2574"
    canvas-height="1209"
    :grid="grid"
  >
    <AtomsFloorLibraryRoomPosition
      :data-user-library="dataUserLibrary"
    ></AtomsFloorLibraryRoomPosition>
    <AtomsFloorEntranceRoomPosition
      :data-user-entrance="dataUserEntrance"
    ></AtomsFloorEntranceRoomPosition>
  </AtomsFloorMainCanvas>
</template>
<script setup lang="ts">
import { grid } from "@/assets/grid-room/first-floor-32";

const dataUserLibrary: { image?: string; name?: string }[] = [
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
];

const dataUserEntrance: { image?: string; name?: string }[] = [
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
  {
    image: undefined,
    name: undefined,
  },
];
</script>
