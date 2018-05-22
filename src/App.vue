<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>Vue Player</h1>
    <div class="test">
      <VideoPlayer :src="src"/>
    </div>
  </div>
</template>

<script>
import VideoPlayer from './components/VideoPlayer'

export default {
  name: 'app',
  data () {
    return {
      src: 'http://download.blender.org/peach/trailer/trailer_400p.ogg'
    }
  },
  components: {
    VideoPlayer
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  border: none;
}

html, body {
  height: 100%;
  width: 100%;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 {
  font-weight: normal;
}

.test {
  width: 400px;
  height: 400px;
}

</style>
