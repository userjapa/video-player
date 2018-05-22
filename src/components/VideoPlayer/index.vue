<template>
  <div class="video-view">
    <div class="full">
      <div class="video full">
        <video :src="src" autoplay/>
      </div>
      <div class="control full"/>
    </div>
  </div>
</template>
<script>
export default {
  name: "video-player",
  props: ['src']
}
</script>
<style lang="scss" scoped>
video {
  width: 100%;
  height: 100%;
}

.full {
  min-width: 100%;
  min-height: 100%;
}

.video-view {
  display: block;
  position: relative;
}

.video, .control {
  position: absolute;
}

.video {
  background-color: #ddd;
}

.control {
  background-color: #000;
  z-index: 10;
}
</style>
