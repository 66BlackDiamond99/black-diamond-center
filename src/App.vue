<template>
  <h1>Black Diamond Center</h1>
  <Container>
    <Video
      videoLink="https://drive.google.com/file/d/11RDzwWZYE66PvU90HKqBG2xsGWf88E5a/preview"
      videoName="Video One"
    />
    <Video
      videoLink="https://drive.google.com/file/d/11RDzwWZYE66PvU90HKqBG2xsGWf88E5a/preview"
      videoName="Video Two"
    />
  </Container>
</template>

<script>
import Video from "./components/Video.vue";
export default {
  name: "App",
  components: { Video },
};
</script>

<style>
* {
  box-sizing: border-box;
  text-align: center;
}
Container {
  display: flex;
  justify-content: center;
  gap: 20px;
}
</style>
