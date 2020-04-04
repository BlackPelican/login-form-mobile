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
  font-weight: 700;
  font-size: 1.8vmin;
  letter-spacing: 0.05vmin;
}
</style>