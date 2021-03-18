<template>
<div> <Head />
  <div class="password-reset">
    <div class="mx-auto form-container">
      <h2>Password Reset</h2>
      <p></p>
      <form >
        <input type="text" class="form-control" name="idnumber" id="" placeholder="Your ID Number">
        <input type="text" class="form-control" name="password" id="" placeholder="Your Email Address">
        <input type="submit" class="btn btn-outline-primary col-xl-12" id="next" value="Submit">
        <p><a href="/login">Go back</a></p>
      </form>
    </div>
  </div>
</div>
</template>

<script>
import Head from './layout/Head'

export default {
  name: 'PasswordReset',
  
  methods: {
  },
  components: {
      Head
  }
}
</script>

<style scoped>
.password-reset {
    text-align: center;
    
  }
.password-reset h2 {
  color: #0074FC;
  margin-bottom: 0px;
}
.password-reset p {
  font-size: 12px;
}


</style>
