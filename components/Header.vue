 <template>
    <div>
      <v-app>
        <v-app-bar app color="white">
          <div class="navbar">
            <nuxt-link to="/">
              <img class="logo" src="http://ui-design-engineering.com/vue/logo.jpg"/>
            </nuxt-link>
            <div class="a-r">   
              <div v-if="$auth.loggedIn">
                {{ $auth.user.username }}
                <v-btn text @click="$auth.logout()">Logout</v-btn>
              </div>
              <div v-else>
                <v-btn text to="/login">Login</v-btn>
                <v-btn text to="/register">Register</v-btn>
              </div>
            </div>
          </div>
        </v-app-bar>     
      </v-app>
    </div>
 </template>

<style scoped lang="scss">
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

 </style>

 
