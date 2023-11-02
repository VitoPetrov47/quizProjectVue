<template>
  <div>
    <Artplayer @get-instance="getInstance" :option="option" :style="style"/>
    <YouTube
        :src="mediaUrl"
        @ready="onReady"
        ref="youtube" />

  </div>
</template>

<script>
import Artplayer from "artplayer/examples/vue/Artplayer";
import YouTube from 'vue3-youtube'

export default {
  data() {
    return {
      option: {
        url: "https://artplayer.org/assets/sample/video.mp4",
      },
      style: {
        width: "600px",
        height: "400px",
        margin: "60px auto 0",
      },
      mediaUrl: 'https://www.youtube.com/watch?v=4dW2KzlYaR4'
    };
  },
  components: {
    Artplayer,
    YouTube
  },
  methods: {
    getInstance(art) {
      console.log(art);
    },
    onReady() {
      this.$refs.youtube.playVideo()
    },
  },
};
</script>