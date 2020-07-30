<template>       
  <div>
     <v-app>
    <v-app-bar app color="white">
      <div class="navbar">
        <nuxt-link to="/">
          <img class="logo" src="http://ui-design-engineering.com/vue/logo.jpg"/>
        </nuxt-link>
        <div class="a-r">   
          <v-btn text to="/">Logout</v-btn>
        </div>
      </div>
    </v-app-bar>   
   
  </v-app>
    <div>
       
                    <nuxt-child />
               
    </div>
  </div>
</template>

<script>
    export default {

       // layout: {videosLayout},

        
     
    }


</script>

<style scoped lang="scss">
.v-application--wrap {
    /* flex: 1 1 auto; */
    /* -webkit-backface-visibility: hidden; */
    /* backface-visibility: hidden; */
    /* display: flex; */
    /* flex-direction: column; */
    min-height: 10vh !important;
    /* max-width: 100%; */
    /* position: relative; */
}
.vid-body, .theme--light.v-application {
  color: #013b30;
  color:#ffffff;
  width:100%;
}
.vid-body {
 
  margin-top:70px;
  h1 {
    margin-left:10px;
  }
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

.index {
    margin-top:-700px;
        h4 {
        margin-left:68px;
    }
}

.listbox-container {
    margin:0 auto;
    position: relative;
    top:-700px;
    max-width:1100px;
    h4 {
    margin-left:68px;
}
.listbox {
    height:210px;
    width:230px;
    padding:2rem 1rem;
    float:left;
    margin:40px 35px; 
    img {
        width:230;
        height:144;
    }
    p {
        color:#013B2F;
        font-size:.89rem;
        line-height:16px;
    }
}
}

.vid-box h5 {
    color:#3DC065;
  }

.v-application a.titles {
    color: #2aba56;
    line-height:10px;
}
.v-application p {
    margin-top: 2px;
}
</style>
