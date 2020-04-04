<template>
  <div class="app-link">{{text}}</div>
</template>

<script>
export default {
  name: "AppLink",
  props: {
    text: String
  }
};
</script>

<style>
.app-link {
  text-decoration: underline;
  color: var(--c-text);
  opacity: 0.8;
  font-size: 1.8vmin;
  letter-spacing: 0.05vmin;
}
</style>