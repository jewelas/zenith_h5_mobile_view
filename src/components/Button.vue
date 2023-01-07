<template>
  <a :href="link" class="link">
    <div class="linkElement">
      <span>
        <img :src="img" :alt="altText" />
      </span>
      <span class="linkText">{{ buttonText }}</span>
    </div>
  </a>
</template>

<script>
export default {
  name: "Button",
  props: ["img", "altText", "buttonText", "link"],
};
</script>

<style scoped>
.link {
  text-decoration: none;
  color: white;
  background-color: #7b61ff;
  border-radius: 4px;
  padding: 11px 20px;
}
.linkElement {
  display: flex;
  justify-content: center;
  align-items: center;
}
.linkText {
  font-weight: 700;
  font-size: 16px;
  line-height: 140%;
  margin-left: 4px;
  text-align: center;
}
</style>
