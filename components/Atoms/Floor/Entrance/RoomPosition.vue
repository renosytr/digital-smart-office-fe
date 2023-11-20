<template>
  <div class="absolute entrance-position z-20">
    <div class="relative w-full h-full">
      <div class="room-name-position left-1/2 bottom-4">ENTRANCE ROOM</div>
      <div class="entrance-space absolute flex">
        <div v-for="(user, index) in props.dataUserEntrance" :key="index">
          <div
            v-if="user.name"
            class="absolute flex flex-col items-center"
            :class="`entrance-chair-${index}`"
          >
            <div
              class="h-16 w-16 rounded-full border-2 p-0.5 bg-white status-active"
            >
              <img
                :src="user.image"
                alt="User Icon"
                class="rounded-full cursor-pointer"
              />
            </div>
            <div
              class="w-24 truncate text-white rounded-xl text-center text-xs py-1 px-2 status-active"
            >
              {{ user.name }}
            </div>
          </div>
          <div
            v-else
            class="absolute flex flex-col items-center h-16 w-16 cursor-pointer translate-x-4 translate-y-5 rounded-lg hover:bg-white hover:opacity-30"
            :class="`entrance-chair-${index}`"
            @click="handleMovePosition"
          ></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import "@/components/Atoms/Floor/Entrance/style.css";
const props = defineProps<{
  dataUserEntrance: { image?: string; name?: string }[];
}>();

const handleMovePosition = () => {};
</script>
