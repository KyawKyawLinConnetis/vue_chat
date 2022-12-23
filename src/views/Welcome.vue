<template>
  <div class="welcome">
    <h1>Welcome dev</h1>
    <div v-if=false>
        <SignUp></SignUp>
        <p>Already member? <span>Login Account?</span></p>
    </div>
    <div v-if=true>
        <Login></Login>
    </div>
  </div>
</template>

<script>
import Login from '../components/Login'
import SignUp from '../components/SignUp'
export default {
  components: {
    Login,
    SignUp 
    },
}
</script>

<style>
    .welcome {
        width: 30%;
        background-color: white;
        margin: 50px auto;
        padding: 5px 50px;
        text-align: center;
        box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
        border-radius: 10px;
    }

    form {
        width: 100%;
        margin: 10px auto;

    }

    form input {
        text-align: center;
        display: block;
        border: 1px solid #efe1ff;
        color: #333;
        margin: 10px auto;
        padding: 10px 20px;
        width: 60%;
        outline-color: #efe1ff;
        border-radius: 10px;
        box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
    }

    form button {
        margin-top: 10px;
        margin-bottom: 10px;
        display: inline-block;
        padding: 7px 15px;
        border-radius: 10px;
        cursor: pointer;
        color: #333;
        background-color: #efe1ff;
        border: 1px solid #efe1ff;
        box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
    }
</style>