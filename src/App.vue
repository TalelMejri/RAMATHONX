<template>
  <div id="app">
    <router-view />
  </div>
</template>
<script>
import AOS from "aos";
export default {
  mounted() {
    AOS.init();
    let test = new SpeechSynthesisUtterance("welcome");
    speechSynthesis.speak(test);
  },
}

</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Nerko+One&display=swap');


* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Nerko One", cursive;
  scroll-behavior: smooth;
}


html {
  overflow-x: hidden;
  scroll-behavior: smooth;
}

*::-webkit-scrollbar {
  width: 5px;
  height: 5px;
}

*::-webkit-scrollbar-track {
  background: #fff;
}

*::-webkit-scrollbar-thumb {
  background: whitesmoke;
  border-radius: 2rem;
}


</style>
