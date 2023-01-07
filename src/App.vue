<template>
  <div class="container">
    <Header />
    <Image />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Image from "./components/Image.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Image,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@500;700&display=swap");
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: "Inter", sans-serif;

  background-image: url("@/assets/background.png"),
    linear-gradient(#130808fd, #141010);
  background-size: cover;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: white;
  height: 100vh;
}
</style>
