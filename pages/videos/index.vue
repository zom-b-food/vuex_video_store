<template>
  <div class="container">
    <div class="listbox-wrapper">
      <h3>Videos</h3>
      <div v-for="video in videos" :key="video.id">
          <div class="listbox">
              <nuxt-link class="titles" :to="`/videos/${video.id}` "><img src="http://ui-design-engineering.com/vue/img-thumb.jpg"/> </nuxt-link>            
              <nuxt-link class="titles" :to="`/videos/${video.id}` "> {{ video.title }} </nuxt-link>          
              <p>
                  {{video.description}}
              </p> 
          </div>
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
        }

    }
</script>

<style scoped lang="scss">

.vid-body, .theme--light.v-application {
  color: #013b30;
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

.listbox-wrapper {
    margin:0 auto;
    position: relative;
    top:-170px;
    left:78px;
    max-width:1100px;
    h3 {
    margin-left:50px;
    color:#3DC065;
}

.listbox {
    height:210px;
    width:230px;
    padding:2rem 1rem;
    float:left;
    margin:35px 35px; 
    img {
        width:230;
        height:144;
        border:8px solid #013B2F;
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

.listbox img:hover {
  border:8px solid #027D61;
  //opacity:.85;
}
</style>
