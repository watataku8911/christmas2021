<template>
  <div class="header-under">
    <!-- <a href="https://watataku-portfolio.web.app" target="_blank">
      <img
        src="@/assets/img_present_special.png"
        alt="present"
        class="present"
      />
    </a>
    <div class="bgElements container">
      <div class="bgElement bgElement--01">
        <img src="@/assets/bg_element_01.png" />
      </div>
      <div class="bgElement bgElement--02">
        <img src="@/assets/bg_element_02.png" />
      </div>
      <div class="bgElement bgElement--03">
        <img src="@/assets/bg_element_03.png" />
      </div>
    </div> -->
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.header-under {
  display: flex;
  align-items: flex-start;
  justify-content: center;
  background-color: #152c4e;
  background-image: url(../../assets/mainimg_bg.png);
  background-repeat: no-repeat;
  background-position: center bottom;
  background-size: contain;
  width: 100%;
  height: 400px;
}

.header-under a {
  z-index: 10;
  display: block;
  width: 125px;
  height: 117px;
  transform: rotate(-5deg);
}

.header-under .present {
  animation: buru 1s infinite 2s;
}

@keyframes buru {
  0% {
    transform: translate(0px, 0px) rotateZ(0deg);
  }
  10% {
    transform: translate(4px, 4px) rotateZ(3deg);
  }
  20% {
    transform: translate(0px, 4px) rotateZ(0deg);
  }
  30% {
    transform: translate(4px, 0px) rotateZ(-3deg);
  }
  40% {
    transform: translate(0px, 0px) rotateZ(0deg);
  }
  100% {
    transform: translate(0px, 0px) rotateZ(0deg);
  }
}

.header-under .present:hover {
  animation: pop 0.5s ease-in-out;
  animation-iteration-count: 1;
}

@keyframes pop {
  0% {
    -moz-transform: translateY(0);
    -ms-transform: translateY(0);
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  50% {
    -moz-transform: translateY(-15%);
    -ms-transform: translateY(-15%);
    -webkit-transform: translateY(-15%);
    transform: translateY(-15%);
  }
  100% {
    -moz-transform: translateY(0);
    -ms-transform: translateY(0);
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
}

/*PC*/
@media screen and (min-width: 1026px) {
  .bgElement--01 {
    position: absolute;
    bottom: 10px;
    left: 30px;
  }

  .bgElement--01 img {
    width: 40px;
  }

  .bgElement--02 {
    position: absolute;
    bottom: 30px;
    right: 60px;
  }

  .bgElement--02 img {
    width: 40px;
  }

  .bgElement--03 {
    position: absolute;
    bottom: 100px;
    left: 150px;
  }

  .bgElement--03 img {
    width: 73px;
  }
}

/*タブレット*/
@media screen and (min-width: 482px) and (max-width: 1025px) {
  .bgElement--01 {
    position: absolute;
    bottom: 10px;
    left: 30px;
  }

  .bgElement--01 img {
    width: 4vw;
  }

  .bgElement--02 {
    position: absolute;
    bottom: 30px;
    right: 60px;
  }

  .bgElement--02 img {
    width: 4vw;
  }

  .bgElement--03 {
    position: absolute;
    bottom: 100px;
    left: 20vw;
  }

  .bgElement--03 img {
    width: 73px;
  }
}
/*スマホ*/
@media screen and (max-width: 481px) {
  .present {
    width: 130px;
  }

  .bgElement--01 {
    position: absolute;
    bottom: 10px;
    left: 30px;
  }

  .bgElement--01 img {
    width: 5vh;
  }

  .bgElement--02 {
    position: absolute;
    bottom: 30px;
    right: 35px;
  }

  .bgElement--02 img {
    width: 5vh;
  }

  .bgElement--03 {
    position: absolute;
    bottom: 100px;
    left: 20vw;
  }

  .bgElement--03 img {
    width: 63px;
  }
}
</style>
