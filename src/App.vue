<template>
  <div id="app">
    <div>
      <img alt="Vue logo" class="background-image" src="/img/backgrounds/beach_long.png" v-bind:style="'height:' + windowHeight + 'px'">
      <div style="background-color:#d4c579;height:150px"/>
      <img src="/img/sharks/shark_dark_blue_reverse.png" class="shark shark2"/>
      <img src="/img/sharks/shark_dark_blue.png" class="shark shark1"/>
      <img src="/img/sharks/shark_dark_blue.png" class="shark shark3"/>
      <img src="/img/sharks/shark_dark_blue_reverse.png" class="shark shark4"/>
      <img id="cloud1" src="img/props/cloud_transparent.png" class="cloud cloud1" />
      <img id="cloud2" src="img/props/cloud_transparent.png" class="cloud cloud2" />
      <img id="cloud3" src="img/props/cloud_transparent.png" class="cloud cloud3" />
      <img id="cloud4" src="img/props/cloud_transparent.png" class="cloud cloud4" />
      <img id="cloud5" src="img/props/cloud_transparent.png" class="cloud cloud5" />
      <img id="cloud6" src="img/props/cloud_transparent.png" class="cloud cloud6" />
      
      <img src="img/props/coconut_tree_transparent.png" class="coconut-tree" />
      <div class="text-container" >
        <div class="d-flex justify-content-center">
        <img src="/img/logos/logo1.png" class="logo" />
        </div>
        <div class="d-flex justify-content-center mt-4">
          <label class="montserrat" style="font-size: 22px;"><b>Worlds first, zero utility, negative value, collectable NFT sharks.</b></label>
        </div>
        <div class="d-flex justify-content-center mt-4">
          <a href="https://twitter.com/SharkpunksNFT" style="text-decoration:none;">
            <div class="hero-button">
              <div class="d-flex justify-content-center px-3">
                <!-- scroll down to how to join -->
                <img class="my-auto" src="/img/logos/twitter_white.png" style="height:24px">
                <label class="m-2 open-sans" style="font-size: 20px;color:white">Twitter</label> 
              </div>
            </div>
          </a>
          <a href="https://discord.com/invite/oh-geez" style="text-decoration:none">
            <div class="hero-button mx-4">
              <div class="d-flex justify-content-center px-3">
                <!-- scroll down to how to join -->
                <img class="my-auto" src="/img/logos/discord_white.png" style="height:20px">
                <label class="m-2 open-sans" style="font-size: 20px;color:white">Discord</label> 
              </div>
            </div>
          </a>
        </div>
      </div>

      <div class="ocean-solid ocean-color"  />
    </div>
    <div class="d-flex justify-content-center" style="width:100%;background-color:#F6ECE5;padding-top:120px;padding-bottom:120px">
      <div class="d-flex justify-content-between my-auto" style="width:70%">
        
        <div class="paragraph-container my-auto mx-5" style="text-align:left">
          <p class="montserrat" style="font-size:24px;font-weight:bold">Future utilization of sharkpunks NFTs may include, but are not limited to:</p>
          <br>
          <p class="mx-3 open-sans">- Decorative painting in the basement of your mother</p>
          <p class="mx-3 open-sans">- Comparison of phallus size</p>
          <p class="mx-3 open-sans">- Companion as you contemplate your existential crisis</p>
        </div>
        <div class="mx-5 my-auto">
          <img v-bind:src="shark" />
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center my-5">
      <div class="my-auto">
        <div class="mx-5">
          <div class="d-flex justify-content-center my-5">
              <img class="my-auto mx-3" src="img/logos/shoyu.png" style="width:50px;height:50px">
              <p class="inter my-auto" style="font-size:36px">SHOYU</p>
            </div>
          <p class="open-sans my-5" style="font-size:22px">Sharkpunks, one of the first NFTs to be listed on Shoyu</p>
          </div>
        </div>
    </div>
    <br>
    <div class="d-flex justify-content-center my-5">
      <div class="d-flex justify-content-end my-auto">
        <div class="mx-5">
          <div class="my-auto mx-5">
            <label class="big-number open-sans">1088</label>
          </div>
          <div class="my-auto">
            <label class="number-description montserrat">total in existence</label>
          </div>
        </div>
        <div class="mx-5">
          <div class="my-auto mx-5">
            <label class="big-number open-sans">750</label>
          </div>
          <div class="my-auto">
            <label class="number-description montserrat">airdropped via raffle</label>
          </div>
        </div>
        <div class="mx-5">
          <div class="my-auto mx-5">
            <label class="big-number open-sans">333</label>
          </div>
          <div class="my-auto">
            <label class="number-description montserrat">to first discord members</label>
          </div>
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center" v-bind:style="'height:' + (0.7* windowHeight) + 'px'" style="background-color:#F2FEDC">
        <div class="my-auto">
          <h1 class="open-sans" ><b>Join our community</b></h1>
          <div class="d-flex justify-content-center my-5">
            <img src="img/logos/twitter.png" class="mx-4" style="width:80px"/>
            <img src="img/logos/discord.png" class="mx-4" style="width:80px"/>
          </div>
        </div>
    </div>



  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      screenWidth: screen.width,
      windowWidth: window.outerWidth,
      windowHeight: window.innerHeight,
      shark: "/img/sharks/1.png",
      cloud1initialX: '200px',
      cloud2nitialX: '300px',
      cloud3initialX: '500px',
      cloud4initialX: '100px',
      cloud5initialX: '600px',
      cloud6initialX: '750px',

    }
  },
  created() {
    window.console.log(this.screenWidth)
    window.console.log(this.windowHeight)
    this.loopImage()

  },
  mounted(){

    document.getElementById('cloud1').style.right = this.cloud1initialX
    document.getElementById('cloud2').style.right = this.cloud2initialX
    document.getElementById('cloud3').style.right = this.cloud3initialX
    document.getElementById('cloud4').style.right = this.cloud4initialX
    document.getElementById('cloud5').style.right = this.cloud5initialX
    document.getElementById('cloud6').style.right = this.cloud6initialX
    document.getElementById('cloud1').style.width = '100px'
    document.getElementById('cloud2').style.width = '200px'
    document.getElementById('cloud3').style.width = '300px'
    document.getElementById('cloud4').style.width = '50px'
    document.getElementById('cloud5').style.width = '60px'
    document.getElementById('cloud6').style.width = '120px'
    this.updateClouds()

    
    // cloud1.style.right
    // window.console.log(cloud1.style)

  },
  methods: {
    loopImage(){
      var i = 0
      setInterval(() => {
        if (i > 16){
          i = 1
        }

        this.shark = "img/sharks/" + i + ".png"
        i = i + 1
      }, 300)
    },
    updateClouds(){
      setInterval(() => {
        var clouds = Array.from(document.getElementsByClassName('cloud'))
        for(var i=0;i<clouds.length;i++){
          var cloud = clouds[i]
          if (parseInt(this.removePx(cloud.style.right)) < -(parseInt(this.removePx(cloud.style.width)))){
            cloud.style.right = this.windowWidth + 'px'
          }
          
          var right = this.removePx(cloud.style.right)
          cloud.style.right = (right - 1) + 'px'
        }


      }, 10)
    },
    removePx(str){
      return str.slice(0, str.length - 2)
    }
  }
}
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Inter&display=swap');
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.montserrat {
  font-family: 'Montserrat', sans-serif;
}

.open-sans {
  font-family: 'Open Sans', sans-serif;
}

.inter {
  font-family: 'Inter', sans-serif;
}

.montserrat-container p{
  font-family: 'Montserrat', sans-serif;
}

.open-sans-container p{
  font-family: 'Open Sans', sans-serif;
}

.inter-container p{
  font-family: 'Inter', sans-serif;
}

.background-image {
  margin-top: 0px;
  top: 0px;
  left: 0px;
}

.shark {
  position: absolute
}

.shark1 {
  width: 100px;
  right: 100px;
  bottom: 50px;
}

.shark2 {
  width: 70px;
  right: 250px;
  bottom: 100px
}
.shark3 {
  width: 40px;
  right: 400px;
  bottom: 200px;
  animation-name:shark-bobble;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}

.shark4 {
  width: 40px;
  right: 450px;
  bottom: 200px;
  animation-name:shark-bobble;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
  animation-delay: 1s;
}

@keyframes shark-bobble {
  0% {transform: translateY(0%);}
  50% {transform: translateY(-20%);}
}



.ocean-solid {
  position:absolute;
  right:350px;
  bottom:180px;
  width: 200px;
  height:40px
}

.cloud {
  position:absolute;
}

.cloud1 {
  right: 200px;
  top: 100px;
  width: 100px;
  animation-name:cloud1-animation;
  animation-duration: 45s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}




.cloud2 {
  right: 300px;
  top: 250px;
  width: 200px;
  animation-name:cloud2-animation;
  animation-duration: 30s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}



.cloud3 {
  right: 500px;
  top: 50px;
  width: 300px;
  animation-name:cloud3-animation;
  animation-duration: 15s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}




.cloud4 {
  right: 100px;
  top: 400px;
  width: 50px;
  animation-name:cloud4-animation;
  animation-duration: 60s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}



.cloud5 {
  right: 600px;
  top: 400px;
  width: 60px;
  animation-name:cloud5-animation;
  animation-duration: 55s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}




.cloud6 {
  right: 750px;
  top: 330px;
  width: 120px;
  animation-name:cloud6-animation;
  animation-iteration-count: infinite;
  animation-duration: 45s;
  animation-timing-function:linear;
}




.logo {
  width: 500px;
}



.hero-button {
  background-color: black;
  border-radius: 10px;
  box-shadow: 0px 0px 8px 3px #74b8cc;
}

.text-container {
  position:absolute;
  top: 130px;
  left:100px
}

.coconut-tree {
  position:absolute;
  left: 150px;
  bottom: 50px;
}


.ocean-color {
  background-color:  #1fcbff
}

.big-number {
  font-size: 60px;
  font-weight: bold;
}

.number-description {
  font-size: 20px
}

.paragraph-container p{
  font-size: 18px

}
</style>
