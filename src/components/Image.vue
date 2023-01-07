<template>
  <div class="imgcontainer">
    <img :src="require('@/assets/' + src)" alt="fuzionx mobile" class="image" />
  </div>
</template>

<script>
export default {
  name: "Image",
  data() {
    return {
      src: "Exchange_zone.png",
      srcs: ["DeFi_zone.png", "Exchange_zone.png"],
    };
  },
  methods: {
    getImgUrl(imgName) {
      return require("../assets/" + imgName);
    },
    callFunction: function () {
      let i = 0;
      setInterval(() => {
        this.src = this.srcs[i];
        if (++i === this.srcs.length) i = 0;
      }, 2000);
    },
  },
  mounted() {
    this.callFunction();
  },
};
</script>

<style scoped>
.imgcontainer {
  margin-top: 50px;
  max-width: 450px;
  max-height: 550px;
}
.image {
  width: 100%;
  height: 100%;
  object-fit: fill;
}
</style>
