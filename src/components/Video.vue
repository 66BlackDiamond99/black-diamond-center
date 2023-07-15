<template>
  <container>
    <videFrame>
      <iframe
        :src="videoLink"
        width="100%"
        height="360"
        allow="fullscreen"
        frameborder="0"
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
  width: 95vw;
  padding: 16px;
}
videFrame {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: relative;
  width: 100%;
  max-width: max-content;
  aspect-ratio: 14/9;
  border-radius: 16px;
  background-color: #212121;
  color: white;
  font-weight: bold;
  overflow: hidden;
  box-shadow: black 0px 2px 15px;
}
img {
  position: absolute;
  width: 58px;
  height: 58px;
  position: absolute;
  right: 1px;
  top: 1px;
}
</style>
