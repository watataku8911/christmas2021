<template>
  <nav class="n-area">
    <ShareTwitter color="white" class="link-twitter" />
    <ShareFacebook color="white" class="link-facebook" />
  </nav>
</template>
<script>
import ShareTwitter from "../components/ShareTwitter";

import ShareFacebook from "../components/ShareFacebook";
export default {
  components: {
    ShareTwitter,
    ShareFacebook
  }
}
</script>
<style scoped>
/*PC*/
@media screen and (min-width: 1026px) {
  .link-twitter {
    position: absolute;
    top: 4vh;
    right: 75px;
    display: block;
    z-index: 10;
  }
  .link-facebook {
    position: absolute;
    top: 4vh;
    right: 35px;
    display: block;
    z-index: 10;
  }
}
/*タブレット*/
@media screen and (min-width: 482px) and (max-width: 1025px) {
  .link-twitter {
    position: absolute;
    top: 2vh;
    right: 45px;
    display: block;
    z-index: 10;
  }
  .link-facebook {
    position: absolute;
    top: 2vh;
    right: 10px;
    display: block;
    z-index: 10;
  }
}
/*スマホ*/
@media screen and (max-width: 481px) {
  .link-twitter {
    position: absolute;
    top: 2vh;
    right: 45px;
    display: block;
    z-index: 10;
  }
  .link-facebook {
    position: absolute;
    top: 2vh;
    right: 10px;
    display: block;
    z-index: 10;
  }
}
</style>
