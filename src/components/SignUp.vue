<template>
  <h1>Sign Up</h1>
  <form @submit.prevent="signUp">
    <input type="text" placeholder="Enter Your Name" v-model="name">
    <input type="email" placeholder="Enter Your Email" v-model="email">
    <input type="password" placeholder="Enter Your Password" v-model="password">
    <button>Sign Up</button>
  </form>
</template>

<script>
import { ref } from '@vue/reactivity'
export default {
  setup() {
    let name = ref("");
    let email = ref("");
    let password = ref("");

    let signUp = () => {
      console.log(name,email,password);
    }

    return {name, email, password, signUp}
  }
}
</script>

<style>

</style>