<template>
  <footer class="footerContainer">
    <Button
      :img="require('@/assets/appstore.svg')"
      altText="app Store"
      buttonText="Apple Store"
      link="https://testflight.apple.com/join/N4GULtOo"
    />
    <Button
      :img="require('@/assets/playstore.svg')"
      altText="play Store"
      buttonText="Play Store"
      link="https://drive.google.com/file/d/1ErcnOcAezOec83rjftv-M04B80K91kyN/view?usp=sharing"
    />
  </footer>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "Footer",
  components: { Button },
};
</script>

<style scoped>
.footerContainer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  min-height: 100px;
  max-height: 100px;
  width: 100%;
  background-color: #000;
  margin-top: 20px;
  padding: 30px;
}
</style>
