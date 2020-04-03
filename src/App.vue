<template>
  <div id="app" class="flex flex--cc">
    <ThePhone />
  </div>
</template>

<script>
import ThePhone from "./components/ThePhone.vue";

export default {
  name: "App",
  components: {
    ThePhone
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Sen:300,400,600,700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --c-bg: #f3f1eb;
  --c-white: #fefdf9;
  --c-text: #333333ee;
}

html,
body {
  position: relative;
  width: 100%;
  height: 100%;
  font-family: "Sen";
}

#app {
  height: 100vh;
  width: 100vw;
  background: var(--c-bg);
}

.flex {
  display: flex;
}

.flex--cc {
  justify-content: center;
  align-items: center;
}

.flex--column {
  flex-direction: column;
}

.h-shadow {
  box-shadow: 0 4px 6px #33333333;
}

.h-rounded {
  border-radius: 3vmin;
}
</style>
