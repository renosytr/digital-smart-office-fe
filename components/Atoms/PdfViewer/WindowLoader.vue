<template>
  <div class="w-screen h-screen">
    <iframe
      id="pdf-js-viewer"
      :src="pathFile"
      title="webviewer"
      frameborder="0"
      width="100%"
      height="100%"
    ></iframe>
  </div>
</template>
<script setup lang="ts">
import { ref } from "vue";
import type { Ref } from "vue";
const pathFile: Ref<string> = ref("lib/pdfjs-4.0.189-dist/web/viewer.html");
</script>
