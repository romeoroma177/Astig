<template>
  <div id="app">
    <div>
      
      
      
    </div>
    <router-view/>
  </div>
</template>

<script>


export default {
  name: 'App',

}
</script>

<style>

*{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

.form-container{
  max-width: 70%;
  
}

input{
    margin: 5px 0px;
}

.psa-logo-ontop {
    width: 30%;
    height: auto;
    margin: 0 10%;
    margin-top: 25%;
}

@media only screen and (min-width: 600px) {
  .psa-logo-ontop {
    width: 20%;
    height: auto;

  }
}

</style>
