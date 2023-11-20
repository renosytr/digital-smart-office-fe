<template>
  <div class="absolute library-position z-20">
    <div class="relative w-full h-full">
      <div class="room-name-position left-1/2 bottom-4">LIBRARY ROOM</div>
      <div class="library-space absolute flex">
        <div v-for="(user, index) in dataUserLibrary" :key="index">
          <div
            v-if="user.name"
            class="absolute flex flex-col items-center"
            :class="`library-chair-${index}`"
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
            :class="`library-chair-${index}`"
            @click="handleMovePosition"
          ></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  dataUserLibrary: any[];
}>();

const handleMovePosition = () => {
  console.log("handle move position");
};
</script>
