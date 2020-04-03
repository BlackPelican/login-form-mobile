<template>
  <input class="form-input" :type="isPassword ? 'password' : 'text'" :placeholder="ph" />
</template>

<script>
export default {
  name: "FormInput",
  props: {
    ph: String,
    isPassword: Boolean
  }
};
</script>

<style>
.form-input {
  border: none;
  border-bottom: 1px solid #ccc;
  height: 5vmin;
  margin-bottom: 10%;
  width: 100%;
  font-size: 2.5vmin;
  color: var(--c-text);
  letter-spacing: 0.1vmin;
}

.form-input::placeholder {
  color: #888;
  font-size: 75%;
}

.form-input:focus {
  outline: none;
}
</style>