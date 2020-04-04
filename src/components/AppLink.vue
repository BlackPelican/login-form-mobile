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
  cursor: pointer;
}

@media (max-width: 1199px) {
  .app-link {
    font-size: 2.7vmin;
  }
}

@media (max-width: 766px) {
  .app-link {
    font-size: 3.6vmin;
  }
}
</style>