<template>
  <div class="button-go flex">
    <h2>{{cta}}</h2>
    <button class="flex flex--cc">
      <img src="../img/arrow.svg" alt="Go" />
    </button>
  </div>
</template>

<script>
export default {
  name: "ButtonGo",
  props: {
    cta: String
  }
};
</script>

<style>
.button-go {
  width: 100%;
  justify-content: space-between;
  align-items: center;
}

.button-go h2 {
  color: var(--c-text);
  font-size: 3vmin;
}

.button-go button {
  height: 10vmin;
  width: 10vmin;
  border-radius: 50%;
  background: linear-gradient(to right, #33353d, #464b55);
  color: #fff;
  border: none;
  cursor: pointer;
  transition: transform 200ms ease-in-out;
}

.button-go button:focus {
  outline: none;
}

.button-go button:active {
  transform: scale(0.95);
}

.button-go button img {
  width: 30%;
}
</style>