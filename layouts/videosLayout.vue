<template>
  <v-app>
    <v-app-bar app color="white">

        
      <div class="navbar">
        <nuxt-link to="/">
          <img class="logo" src="http://ui-design-engineering.com/vue/logo.jpg"/>
        </nuxt-link>
        <div class="fr">   
         
          <div>
            <v-btn text to="/">Logout</v-btn>
          </div>
<!-- 
<v-btn text to="/login">Login</v-btn>
            <v-btn text to="/register">Register</v-btn> -->
         
        </div>
      </div>
    </v-app-bar>   
    <div id="store-body" class="container">
      <nuxt-child />
    </div>
  </v-app>
</template>

<script>

</script>

<style scoped lang="scss">
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 14px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

#store-body {
  color: #013b30;
  background-color:#ffffff;
  margin-top:70px;
  h1 {
    margin-left:10px;
  }
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.theme--light.v-application {
  color: #013b30;
  background-color:#ffffff;
}

.container {
  min-height: 75vh !important;
  text-align: left;
  max-width:1000px;
  margin:0 auto;
}

.container > .center {
  text-align:center;
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
.fr {
  text-align:right;
}

#index h4 {
    margin-left:68px;
}

</style>
