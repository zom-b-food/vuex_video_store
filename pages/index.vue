<template>
<div>
   <Header />
    <div>   
      <div class="container">
          <div class="card">
              <h4 class="title">
                vuex_video_store
              </h4>
              <p>I approached this project as a user story and it's several tasks with the estimated time expectation of 3 hours. And since I 
                received this error: <small>Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists</small> , performing git clone to the starter templates was not possible so I built what you see here from scratch. I 
                confess to going over the time expectation by 1 hour as I'm much more familiar with Angular than I am with VUEX/NUXT. In any
                event, I'm confident all tasks could be completed and a few kinks ironed out given another hour or so.  </p>
                <p>Evidence of all other required skills can be viewed in my development sandbox at http://uiuxsandbox.com and many other of my 
                  URLs listed on my cover letter.</p>
                <p>Thank you,<br/>Adam L. Marsh</p>
                <br/>
                <p>$ git clone https://github.com/zom-b-food/vuex_video_store</p>
                <p><small>Cover letter for this position:<br/> https://docs.google.com/document/d/16ns67eH_sD0AWJO5VrYWTPuWIjhh4rM-lnkK1hgc440/edit<br/>
                Introductory Video:<br/> http://ui-design-engineering.com/AM-intro.mp4</small></p>
              <div class="links">
                <a
                  href="/register"
                  rel="noopener noreferrer"
                  class="btn-orange"
                >
                  Let's Go!
                </a>   
              </div>
          </div>
        <div>
      </div>
    </div>
  </div>
</div>
</template>
<!-- The core Firebase JS SDK is always required and must be listed first -->
<script src="/__/firebase/7.17.1/firebase-app.js"></script>

<!-- TODO: Add SDKs for Firebase products that you want to use
     https://firebase.google.com/docs/web/setup#available-libraries -->
<script src="/__/firebase/7.17.1/firebase-analytics.js"></script>

<!-- Initialize Firebase -->
<script src="/__/firebase/init.js"></script>
<script>
import Header from '@/components/Header'

export default {
    head: {
            title: 'Welcome to VueX-Nuxt Video List'
        },
    components: {
      Header
      }
    }
</script>

<style lang="scss">

.v-application--wrap {
    min-height: 23vh !important;
}

.card {
  margin-top:-88px;
  background-color:rgba(255,255,255,.9);
  height:600px;
  width:800px;
  color:black;
  padding:2rem 1.5rem;
  margin: 0 auto;
  text-align:center;
  p {
    text-align:left;
  }
}

.navbar {
  width:100%;
  height:66px;
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

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 800;
  font-size: 2rem;
  color: #35495e;
  letter-spacing: 1px;
}

a.btn-orange {
    display: inline-block;
    margin-bottom: 0;
    font-weight: 800;
    text-align: center;
    white-space: nowrap;
    vertical-align: middle;
    -ms-touch-action: manipulation;
    touch-action: manipulation;
    cursor: pointer;
    background-image: none;
    color:orange;
    border: 1px solid orange;
    padding: 6px 12px;
    font-size: 14px;
    line-height: 1.42857143;
    border-radius: 4px;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    user-select: none;
}
</style>
