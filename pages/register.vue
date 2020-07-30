<template>
<div>
 <Header />
 <div class="store-body">
<div class="container">
  
 
    <div id="index">
        <h4>Register</h4>
        <div class="card">
         <br/>
       <UserAuthForm buttonText="Register" :submitForm="registerUser" hasName="true" /> 
    </div>
  </div>
</div>
</div>
</div>
</template>

<script>
import Header from '@/components/Header'
   
   import UserAuthForm from '@/components/UserAuthForm'
    
    export default {
      components: {
          Header,
          UserAuthForm
      }, 
      methods: {
          registerUser(registrationinfo) {
             
          }
      }
    }

</script>

<style scoped lang="scss">
.store-body {
    margin-top: 70px;
    background-color: #013b30;
    color: #ffffff;
    width: 100%;
    min-height: 100vh;
    margin-top: -836px !important;
}

.v-messages__message {
    color: red !important;
}

.store-body, .theme--light.v-application {
  background-color: #013b30;
  color:#ffffff;
  width:100%;
}

.navbar {
  width:100%;
  max-width:908px;
  margin:0 auto;
  img.logo {
    height:55px;
    float:left;
  }
}

.a-r {
  text-align:right;
}

.card {
  background-color:rgba(255,255,255,.9);
  height:300px;
  width:400px;
  color:black;
  padding:2rem 1.5rem;
  margin: 0 auto;
}

#index h4 {
  margin-left: 240px;
  padding-top: 220px;
}
</style>
