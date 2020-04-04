<template>
  <div class="app-button flex">
    <h2>{{cta}}</h2>
    <button class="flex flex--cc h-shadow">
      <img src="../img/arrow.svg" alt="Go" />
    </button>
  </div>
</template>

<script>
export default {
  name: "AppButton",
  props: {
    cta: String
  }
};
</script>

<style>
.app-button {
  width: 100%;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 6vmin;
}

.app-button h2 {
  color: var(--c-text);
  font-size: 3vmin;
}

.app-button button {
  height: 9vmin;
  width: 9vmin;
  border-radius: 50%;
  background: linear-gradient(to right, #33353d, #464b55);
  color: #fff;
  border: none;
  cursor: pointer;
  transition: transform 200ms ease-in-out;
}

.app-button button:focus {
  outline: none;
}

.app-button button:active {
  transform: scale(0.95);
}

.app-button button img {
  width: 30%;
}

@media (max-width: 1199px) {
  .app-button button {
    width: 13.5vmin;
    height: 13.5vmin;
  }

  .app-button h2 {
    font-size: 4.5vmin;
  }
}

@media (max-width: 766px) {
  .app-button button {
    width: 18vmin;
    height: 18vmin;
  }

  .app-button h2 {
    font-size: 6vmin;
  }
}
</style>