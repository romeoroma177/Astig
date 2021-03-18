<template>
  <div class="login">
    <Head />
    <div class="mx-auto form-container">
      <h2>Login</h2>
      <p>Sign in to your account</p>
      <form >
        <input type="text" class="form-control" name="idnumber" id="" placeholder="Your ID Number">
        <input type="text" class="form-control" name="password" id="" placeholder="Your Password">
        <input type="submit" @click.prevent="toHome()" class="btn btn-outline-primary col-xl-12" value="Login">
        <p><a href="/passwordreset"> Forgot Password </a></p>
        <input type="button" @click.prevent="toRegister()" class="btn btn-outline-secondary col-xl-12" value="Register New Account">
      </form>
    </div>
  </div>
</template>

<script>
import Head from './layout/Head'

export default {
  name: 'Login',
  
  methods: {
    toRegister() {
      this.$router.push('/register')
    },
    toHome() {
      this.$router.push({path: 'dataentry'})
    }
  }, 
  components: {
    Head
  }
}
</script>

<style scoped>
.login {
    text-align: center;
    
  }
.login h2 {
  color: #0074FC;
  margin-bottom: 0px;
}
.login p {
  font-size: 12px;
  margin: 0;
}


</style>
