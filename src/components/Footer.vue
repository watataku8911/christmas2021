<template>
  <footer>
    <div class="footer-top"></div>
    <div class="footer-under">
      <div class="sns">
        <ShareFacebook color="black" class="footer-link-facebook" />
        <div class="module--spacing--very--small"></div>
        <ShareTwitter color="black" class="footer-link-twitter" />
      </div>
      <small
        ><a href="https:watataku-portfolio.web. app" target="_blank"
          >&copy;2021 Watataku.</a
        ></small
      >
    </div>
  </footer>
</template>

<script>
import ShareTwitter from "../components/ShareTwitter";

import ShareFacebook from "../components/ShareFacebook";
export default {
  components: {
    ShareTwitter,
    ShareFacebook,
  },
};
</script>

<style scoped>
.module--spacing--very--small {
  height: 5px;
}

footer {
  height: 55vh;
  width: 100%;
}

.footer-top {
  height: 30vh;
  background-color: #000;
  background-image: url(../assets/footer_bg.png);
  background-size: cover;
  background-position: left bottom;
}

.footer-under {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 25vh;
}

.sns {
  position: absolute;
  bottom: 3vh;
  right: 3vh;
}

small {
  font-size: 1em;
  letter-spacing: 2px;
}

small a {
  color: #000;
  text-decoration: none;
}
</style>
