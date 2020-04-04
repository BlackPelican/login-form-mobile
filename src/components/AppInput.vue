<template>
  <input class="app-input" :type="isPassword ? 'password' : 'text'" :placeholder="ph" />
</template>

<script>
export default {
  name: "AppInput",
  props: {
    ph: String,
    isPassword: Boolean
  }
};
</script>

<style>
.app-input {
  border: none;
  border-bottom: 1px solid #ccc;
  height: 5vmin;
  margin-bottom: 10%;
  width: 100%;
  font-size: 2.6vmin;
  color: var(--c-text);
  letter-spacing: 0.1vmin;
}

.app-input::placeholder {
  color: #888;
  font-size: 75%;
}

.app-input:focus {
  outline: none;
}

@media (max-width: 1199px) {
  .app-input {
    font-size: 3.9vmin;
  }
}

@media (max-width: 766px) {
  .app-input {
    font-size: 5.2vmin;
  }
}
</style>