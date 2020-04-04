<template>
  <section id="the-sign-in" class="flex flex--column">
    <h1 :class="{'h-fade-in': true}">Welcome Back</h1>
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

.h-fade-in {
  animation: fade-in;
  animation-duration: 2000ms;
  animation-timing-function: ease-in-out;
}

.h-fade-left {
  animation: fade-left;
  animation-duration: 2000ms;
  animation-timing-function: ease-in-out;
}

.wrap--links {
  justify-content: space-between;
  width: 100%;
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: scale(0.9);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

@keyframes fade-left {
  0% {
    transform: translateX(-150%);
  }

  100% {
    transform: translateX(0);
  }
}
</style>