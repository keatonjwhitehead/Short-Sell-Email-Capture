<template>
  <div>
  <!-- <div class="container-fluid m-0 p-0">
    <div id="home-page" class="full-height">
       <video v-bind:src="video" autoplay="true" loop="true" type="video/mp4"> click here</video>"

      <div class="v-header container">
        <div class="fullscreen-video-wrap">
          <video autoplay muted loop id="myVideo">
            <source src="../assets/background_video.mp4" type="video/mp4">
          </video>
        </div>
      </div>
      <div class="header-overlay"></div>
      <div class="header-content text-md-center">
        <h1>Welcome Everyone</h1>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Id temporibus perferendis necessitatibus numquam amet impedit explicabo? Debitis quasi ullam aperiam!</p>
        <a class="btn">Find Out More</a>
      </div>
     </div>
    <div id="about" class="bg-warning p-4"> </div>
    <div id="contact" class="bg-info p-4"> </div>
    <div id="footer" class="bg-primary p-4"> </div>
  </div> -->

  <header class="v-header container">
    <div class="fullscreen-video-wrap">
      <!--  https://www.videvo.net/video/typing-on-computer-white-bg/4475/ -->
      <!-- DO NOT USE THIS VIDEO, I JUST NEEDED A HOSTED VIDEO FOR THIS CODEPEN> USE THE ONE ABOVE -->
      <video src="../assets/background_video.mp4" autoplay="true" loop="true">
    </video>
    </div>
    <div class="header-overlay"></div>
    <div class="header-content text-md-center">
      <h1>Welcome Everyone</h1>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Id temporibus perferendis necessitatibus numquam amet impedit explicabo? Debitis quasi ullam aperiam!</p>
      <a class="btn">Find Out More</a>
    </div>
  </header>

</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      video: '../assets/background_video.mp4'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* #home-page {
  background: url('../assets/background_video.mp4') no-repeat center center;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  backgroun-size: cover;
}
.v-header{
  height:100vh;
  display:flex;
  align-items:center;
  color:#fff;
}
.container {
  max-width: 960px;
  padding-left: 1rem;
  padding-right: 1rem;
  margin: auto;
  text-align:center;
}
.fullscreen-video-wrap{
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100vh;
  overflow:hidden;
}
.fullscreen-video-wrap video {
  min-width: 100%;
  min-height: 100%;
}
.header-overlay{
  height:100vh;
  width:100vw;
  position: absolute;
  top:0;
  left:0;
  background:#25470

} */

*{
  box-sizing: border-box;
}

body{
  margin:0;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size:1rem;
  font-weight:normal;
  line-height:1.5;
  color:#333;
  overflow-x:hidden;
}

.v-header{
  height:100vh;
  display:flex;
  align-items:center;
  color:#fff;
}

.container{
  max-width:960px;
  padding-left:1rem;
  padding-right:1rem;
  margin:auto;
  text-align:center;
}

.fullscreen-video-wrap{
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100vh;
  overflow:hidden;
}

.fullscreen-video-wrap video{
  min-height:100%;
  min-width:100%;
}

.header-overlay{
  height:100vh;
  position: absolute;
  top:0;
  left:0;
  width:100vw;
  z-index:1;
  background:#225470;
  opacity:0.85;
}

.header-content{
  z-index:2;
}

.header-content h1{
  font-size:50px;
  margin-bottom:0;
}

.header-content p{
  font-size:1.5rem;
  display:block;
  padding-bottom:2rem;
}

.btn{
  background: #34b3a0;
  color:#fff;
  font-size:1.2rem;
  padding: 1rem 2rem;
  text-decoration: none;
}

.section{
  padding:20px 0;
}

.section-b{
  background:#333;
  color:#fff;
}

@media(max-width:960px){
  .container{
    padding-right:3rem;
    padding-left:3rem;
  }
}
</style>
