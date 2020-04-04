<template>
  <section id="the-sign-in" class="flex flex--column">
    <TheBackground />
    <h1 class="a-fade-in">Welcome Back.</h1>
    <AppInput class="a-fade-in" ph="Email" />
    <AppInput class="a-fade-in" ph="Password" isPassword />
    <AppButton class="a-fade-in" cta="Sign in" />
    <div class="wrap--links flex a-fade-in">
      <AppLink text="Sign up" />
      <AppLink text="Reset Password" />
    </div>
  </section>
</template>

<script>
import AppInput from "./AppInput.vue";
import AppButton from "./AppButton.vue";
import AppLink from "./AppLink.vue";
import TheBackground from "./TheBackground";

export default {
  name: "TheSignIn",
  components: {
    AppInput,
    AppButton,
    AppLink,
    TheBackground
  }
};
</script>

<style>
#the-sign-in {
  height: 100%;
  width: 100%;
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
  z-index: 3;
}

.a-fade-in {
  animation: fade-in;
  animation-duration: 1000ms;
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

@media (max-width: 1199px) {
  #the-sign-in h1 {
    font-size: 6vmin;
  }
}

@media (max-width: 766px) {
  #the-sign-in h1 {
    font-size: 8vmin;
  }
}
</style>