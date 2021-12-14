<template>
  <div class="header-under">
    <div class="present-box">
      <Chip msg="アーカイブ" v-show="isOpen" />
      <div class="module--spacing"></div>
      <a href="https://watataku8911.github.io/christmas2020/" target="_blank">
        <img
          src="@/assets/img_present_special.png"
          alt="present"
          class="present"
          @mouseover="mouseover"
          @mouseleave="mouseleave"
        />
      </a>
    </div>
  </div>
</template>

<script>
import Chip from "../Chip.vue";
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  components: {
    Chip,
  },
  methods: {
    mouseover() {
      this.isOpen = true;
    },

    mouseleave() {
      this.isOpen = false;
    },
  },
};
</script>

<style scoped>
.module--spacing {
  height: 15px;
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
  .present-box {
    position: absolute;
    bottom: 20%;
    left: 63%;
    text-align: center;
    transform: rotate(-5deg);
  }

  a {
    display: block;
  }

  .present {
    animation: buru 1s infinite 2s;
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
  .present-box {
    position: absolute;
    bottom: 15%;
    left: 60%;
    text-align: center;
    transform: rotate(-5deg);
  }

  a {
    display: block;
  }

  .present {
    width: calc(5vh + 10vw);
    animation: buru 1s infinite 2s;
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
  .present-box {
    position: absolute;
    bottom: 0%;
    left: 60%;
    text-align: center;
    transform: rotate(-5deg);
  }

  a {
    display: block;
  }

  .present {
    width: 80px;
    animation: buru 1s infinite 2s;
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
</style>
