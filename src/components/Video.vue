<template>
  <container>
    <videFrame>
      <iframe
        :src="videoLink"
        width="640"
        height="360"
        allow="fullscreen"
        frameborder="0"
        scrolling="no"
        seamless
      >
      </iframe>
      <img src="../assets/logo.png" />
      {{ videoName }}
    </videFrame>
  </container>
</template>

<script>
export default {
  name: "Video",
  props: {
    videoLink: String,
    videoName: String,
  },
};
</script>

<style scoped>
container {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 650px;
  padding: 16px;
}
videFrame {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  width: 640px;
  border-radius: 16px;
  background-color: #212121;
  color: white;
  font-weight: bold;
  overflow: hidden;
  box-shadow: black 0px 2px 15px;
}
img {
  position: absolute;
  width: 64px;
  height: 64px;
  position: absolute;
  right: 0px;
  top: 0px;
}
</style>
