<template>
  <section id="the-sign-in" class="flex flex--column">
    <h1>Welcome Back</h1>
    <AppInput ph="Email" />
    <AppInput ph="Password" isPassword />
    <AppButton cta="Sign in" />
    <div class="wrap--links flex">
      <AppLink text="Sign up" />
      <AppLink text="Reset Password" />
    </div>
  </section>
</template>

<script>
import AppInput from "./AppInput.vue";
import AppButton from "./AppButton.vue";
import AppLink from "./AppLink.vue";

export default {
  name: "TheSignIn",
  components: {
    AppInput,
    AppButton,
    AppLink
  }
};
</script>

<style>
#the-sign-in {
  height: 100%;
  width: 100%;
  background-image: url("../img/bg01.svg");
  background-size: contain;
  background-repeat: no-repeat;
  align-items: flex-start;
  justify-content: space-between;
  padding: 40% 10% 10% 10%;
  position: relative;
}

#the-sign-in h1 {
  font-size: 4vmin;
  max-width: 10ch;
  height: 4vmin;
  font-weight: 400;
  color: #fff;
  margin-bottom: 80%;
}

.wrap--links {
  justify-content: space-between;
  width: 100%;
}
</style>