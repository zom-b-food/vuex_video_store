<template>
<div>
  
   <div class="vid-component">
    <div class="container">
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

.vid-component {
   margin:0 auto;
    position: relative;
    margin-top:565px;
    left:-132px;
    max-width:1100px;
    h3 {
    margin-left:100px;
    color:#3DC065;
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
