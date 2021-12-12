<template>
  <div class="header-top">
    <Navigation />
    <h1 class="header-top-title">
      Watataku's<br />
      X'mas special site at 2021
    </h1>
  </div>
</template>

<script>
import Navigation from "../Navigation";

export default {
  components: {
    Navigation,
  },
};
</script>

<style scoped>
/*PC*/
@media screen and (min-width: 1026px) {
  .header-top {
    background-color: #263c5f;
    width: 100%;
    height: 500px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .header-top .header-top-title {
    z-index: 20;
    color: #999;
    letter-spacing: 1px;
    font-size: 5.5em;
    font-weight: bold;
    font-family: "Kaushan Script", cursive;
    font-family: "Bad Script", cursive;
  }
}

/*タブレット*/
@media screen and (min-width: 482px) and (max-width: 1025px) {
  .header-top {
    background-color: #263c5f;
    width: 100%;
    height: 60vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .header-top .header-top-title {
    z-index: 10;
    color: #999;
    font-size: calc(4.5vw + 1.5em);
    font-weight: bold;
    font-family: "Kaushan Script", cursive;
    font-family: "Bad Script", cursive;
  }
}
/*スマホ*/
@media screen and (max-width: 481px) {
  .header-top {
    padding-top: 50%;
    background-color: #263c5f;
    width: 100%;
    display: flex;
    justify-content: center;
    height: 10px;
  }

  .header-top .header-top-title {
    color: #999;
    letter-spacing: 1px;
    font-size: 1.8em;
    font-weight: bold;
    font-family: "Kaushan Script", cursive;
    font-family: "Bad Script", cursive;
  }
}
</style>
