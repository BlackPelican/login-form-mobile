<template>
  <div class="the-background">
    <img class="img--yellow" src="../img/yellow.svg" alt="." />
    <img class="img--black" src="../img/black.svg" alt="." />
    <img class="img--blue" src="../img/blue.svg" alt="." />
  </div>
</template>

<script>
export default {
  name: "TheBackground"
};
</script>

<style>
.the-background {
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  z-index: 0;
}

.the-background img {
  height: initial;
  position: absolute;
  top: 0;
  left: 0;
}

.img--yellow {
  z-index: 2;
  width: 70%;
  animation: a-black 1000ms;
}

@keyframes yellow {
  0% {
    transform: translate(-100%, -100%);
  }
  100% {
    transform: translate(0, 0);
  }
}

.img--black {
  z-index: 1;
  animation: a-black 1000ms;
}

@keyframes a-black {
  0% {
    transform: translate(-100%, -100%) rotate(-20deg);
  }
  100% {
    transform: translate(0, 0) rotate(0);
  }
}

.img--blue {
  z-index: 0;
  animation: a-blue 1000ms;
}

@keyframes a-blue {
  0% {
    transform: translate(100%, -100%) rotate(20deg);
  }
  100% {
    transform: translate(0, 0) rotate(0);
  }
}
</style>