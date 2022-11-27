<template>
  <h1>Login</h1>
  <form @submit.prevent="login">
    <input type="text" placeholder="Enter Your Name" v-model="name">
    <input type="password" placeholder="Enter Your Password" v-model="password">
    <button>Sign In</button>
  </form>
</template>

<script>
import { ref } from '@vue/reactivity';
export default {
    setup() {
        let name = ref("");
        let password = ref("");

        let login = () => {
        console.log(name.value,password.value);
        }

        return {name, password, login}
    }
}
</script>

<style>

</style>