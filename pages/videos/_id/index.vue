<template>
<div class="store-body">
  <div class="container">
    <h3 class="title">Video Player</h3> 
       <div id="back">
          <nuxt-link class="back" :to="`/videos/`">
            Back
          </nuxt-link>
        </div> 
        <img src="http://ui-design-engineering.com/vue/img-back.jpg"/>   
        <div class="vid-box">   
          <h5 id="sub-title">
            {{ video.title }}  
          </h5>
          <p>  
            {{ video.description }}
          </p>     
        </div>
  </div>
</div>
</template>

<script>
    export default {
        props: ['video']
    }

</script>

<style lang="scss">
.v-application--wrap {
    min-height: 35vh !important;
}

.store-body {
  position:relative;
  margin-top:-550px;
  margin-left:40%;
 
  
}
 h3.title {
   position: absolute;
    margin-top: -197px;
    margin-left: -182px;
  }
#back {
  position:relative;
  margin-left:-100px;
  margin-top:-60px;
  a.back {
  font-weight: 800;
  color:#013B30;
  text-decoration:underline;
  font-size: .89rem;
 }
}

.v-application a.black {
  font-weight: 800;
  color:black;
}

// #vid-component {
//   height:365;
//   width:579px;
//   padding:0;
//   margin-left: 12rem;
//   margin-top:-260px;
// }

// .vid-box {
//   margin-top:10px;
// }

h5, h3 {
  color:#3DC065;
 
}
</style>
