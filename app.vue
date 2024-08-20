<script setup lang="ts">
useHead({
  title: '3D App',
  script: [
    { src: 'https://ajax.googleapis.com/ajax/libs/model-viewer/3.5.0/model-viewer.min.js', type: 'module' },
  ]
})
</script>

<template>
  <div class="container">

    <model-viewer
      alt="Neil Armstrong's Spacesuit from the Smithsonian Digitization Programs Office and National Air and Space Museum"
      src="content.glb" ar shadow-intensity="1" camera-controls touch-action="pan-y"
      style="width: 100%; height: 100%;" />
  </div>
</template>

<style scoped>
.container {
  width: 90vw;
  height: 90vh;
}
</style>
