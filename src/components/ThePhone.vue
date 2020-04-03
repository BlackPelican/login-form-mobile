<template>
  <main id="the-phone" class="h-shadow h-rounded">
    <TheSignIn />
  </main>
</template>

<script>
import TheSignIn from "./TheSignIn.vue";
export default {
  name: "ThePhone",
  components: {
    TheSignIn
  }
};
</script>

<style scoped>
#the-phone {
  height: 80vh;
  width: calc(80vh / 2.1);
  background: var(--c-white);
  overflow: hidden;
}
</style>