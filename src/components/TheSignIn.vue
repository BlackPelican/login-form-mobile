<template>
  <section id="the-sign-in" class="flex flex--column">
    <h1>Welcome Back</h1>
    <FormInput ph="Email" />
    <FormInput ph="Password" isPassword />
    <ButtonGo cta="Sign in" />
  </section>
</template>

<script>
import FormInput from "./FormInput.vue";
import ButtonGo from "./ButtonGo.vue";

export default {
  name: "TheSignIn",
  components: {
    FormInput,
    ButtonGo
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
  justify-content: flex-start;
  padding: 40% 10% 10% 10%;
}

#the-sign-in h1 {
  max-width: 10ch;
  height: 4vmin;
  font-weight: 400;
  color: #fff;
  margin-bottom: 80%;
}
</style>