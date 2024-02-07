<script>
export default {
  data() {
    return {
      imgName: ["img01.png", "img02.png"],
    };
  },

  methods: {
    getImgUrl(imageName) {
      return new URL(`../assets/${imageName}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <hero>
    <img :src="getImgUrl(image)" alt="" v-for="image in imgName" />
  </hero>
</template>
