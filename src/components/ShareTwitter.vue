<template>
  <p>
    <a
      href="https://twitter.com/share?url=https://watataku8911.github.io/christmas2020/&text=x'mas special site"
      target="_blank"
      class="share-link"
    >
      <TwitterSvgBlack v-if="this.color == 'black'" />
      <TwitterSvgWhite v-else />
    </a>
  </p>
</template>

<script>
import TwitterSvgBlack from "@/assets/icon/icon_twitter_black.svg";
import TwitterSvgWhite from "@/assets/icon/icon_twitter_white.svg";
export default {
  props: {
    color: {
      type: String,
      required: true,
    },
  },
  components: {
    TwitterSvgBlack,
    TwitterSvgWhite,
  },
};
</script>

<style scoped>
.share-link {
  width: 32px;
  height: 32px;
}

.share-link:hover {
  display: block;
  transform: scale(1.3, 1.3);
  -webkit-transform: scale(1.3, 1.3);
  -moz-transform: scale(1.3, 1.3);
}
</style>
