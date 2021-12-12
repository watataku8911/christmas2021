<template>
  <div class="header-under">
    <img src="@/assets/img_present_special.png" alt="present" class="present" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
};
</script>

<style scoped>
/*PC*/
@media screen and (min-width: 1026px) {
  .present {
    position: absolute;
    bottom: 20%;
    left: 60%;
  }

  .header-under {
    background-color: #263c5f;
    background-image: url(../../assets/mainimg_bg.png);
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: contain;
    width: 100%;
    height: 300px;
  }
}

/*タブレット*/
@media screen and (min-width: 482px) and (max-width: 1025px) {
  .present {
    position: absolute;
    bottom: 20%;
    left: 60%;
    transform: rotate(-5deg);
  }

  .header-under {
    background-color: #263c5f;
    background-image: url(../../assets/mainimg_bg.png);
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: contain;
    width: 100%;
    height: 150px;
  }
}
/*スマホ*/
@media screen and (max-width: 481px) {
  .present {
    width: 60px;
    position: absolute;
    bottom: 0%;
    left: 60%;
  }

  .header-under {
    background-color: #263c5f;
    background-image: url(../../assets/mainimg_bg.png);
    background-repeat: no-repeat;
    background-position: center bottom;
    background-size: contain;
    width: 100%;
    height: 400px;
  }
}
</style>
