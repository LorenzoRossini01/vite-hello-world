<script>
export default {
  data() {
    return {
      imgName: "img01.png",
    };
  },

  methods: {
    getImgUrl(img) {
      return new URL(`../assets/${img}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div>
    <img src="../assets/img01.png" alt="" />
  </div>
</template>

<style></style>
