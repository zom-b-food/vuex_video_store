<template>
<div>
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
        </div>
      </div>
    </v-app-bar>    
  </v-app>
  <div> 
    <div id="vid-component">
      <nuxt-child :video="video" />
    </div>
  </div>
</div>
</template>

<script>
    export default {
        asyncData() {
            return {       
                videos: [
                    {
                    "id": 1,
                    "title": "What It's Like To Work At AlgaeCal",
                    "description": "Discover what it's like to work at AlgaeCal with this quick video!",
                    "video_id": "m3ralniniq"
                    },
                    {
                    "id": 2,
                    "title": "Esther Mangini Testimonial",
                    "category": "Testimonials",
                    "description": "Esther's journey to healthier bones",
                    "video_id": "ybyot0dm7q"
                    },
                    {
                    "id": 3,
                    "title": "Teresa Cucurull Testimonial",
                    "description": "Teresa's journey to healthier bones",
                    "video_id": "mhmv73k989"
                    },
                    {
                    "id": 4,
                    "title": "Perfect Pilates For Osteoporosis - Legwork",
                    "description": "Bone Healthy Exercises!",
                    "video_id": "3n5p02h26w"
                    },
                    {
                    "id": 5,
                    "title": "Perfect Pilates For Osteoporosis - Amazing Abs",
                    "description": "Bone Healthy Exercises!",
                    "video_id": "kkgeu7v2va"       
                    },
                    {
                    "id": 6,
                    "title": "Lara's Homemade Granola",
                    "description": "Bone Healthy Recipes",
                    "video_id": "m6amjftj3w"
                    },
                    {
                    "id": 7,
                    "title": "Brazil Nut Pesto",
                    "description": "Bone Healthy Recipes",
                    "video_id": "ajoe5d0jk0"
                    }
                ]
            }   
        },
 computed: {
      video() {
        return this.videos.find(v => v.id == this.$route.params.id)
      }
    }
  }
</script>

<style scoped lang="scss">
.v-application--wrap {
    min-height: 10vh !important;
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

#back {
  position:relative;
  margin-left:-100px;
  margin-top:-160px;
  a.back {
  font-weight: 800;
  color:#013B30;
  text-decoration:underline;
  font-size: .89rem;
  }
  h5, h3 {
  color:#3DC065;
  }
}

.v-application a.black {
  font-weight: 800;
  color:black;
}

#vid-component {
  height:365;
  width:579px;
  padding:0;
  margin-left: 12rem;
  margin-top:260px;
}

.vid-box {
  margin-top:10px;
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
