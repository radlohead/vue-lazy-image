<template>
  <div class="root">
    <h1>lazy image</h1>

    <template>
      <v-lazy-image
        src="http://lorempixel.com/400/200/"
        src-placeholder="https://cdn-images-1.medium.com/max/80/1*xjGrvQSXvj72W4zD6IWzfg.jpeg"
      ></v-lazy-image>
    </template>
  </div>
</template>

<script>
import VLazyImage from "v-lazy-image";

export default {
  name: "HelloWorld",
  data() {
    return {};
  },
  components: {
    VLazyImage
  }
};
</script>

<style scoped>
.v-lazy-image {
  width: 100%;
  max-width: 300px;
  filter: blur(10px);
  transition: filter 0.7s;
}
.v-lazy-image-loaded {
  filter: blur(0);
}
</style>
