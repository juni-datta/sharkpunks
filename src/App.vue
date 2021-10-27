<template>
  <div id="app">
    <div>
      <img alt="Vue logo" class="background-image" src="/img/backgrounds/beach_long.png" v-bind:style="'height:' + windowHeight + 'px'">
      <div style="background-color:#d4c579;height:150px"/>
      <img src="/img/sharks/3.png" class="shark shark2"/>
      <img src="/img/sharks/4.png" class="shark shark1"/>
      <img src="/img/sharks/2.png" class="shark shark3"/>
      <img src="/img/sharks/16.png" class="shark shark4"/>
      <img src="/img/sharks/3.png" class="shark shark5"/>
      <img src="/img/sharks/7.png" class="shark shark6"/>
      <img id="cloud1" src="img/props/cloud_transparent.png" class="cloud cloud1" />
      <img id="cloud2" src="img/props/cloud_transparent.png" class="cloud cloud2" />
      <img id="cloud3" src="img/props/cloud_transparent.png" class="cloud cloud3" />
      <img id="cloud4" src="img/props/cloud_transparent.png" class="cloud cloud4" />
      <img id="cloud5" src="img/props/cloud_transparent.png" class="cloud cloud5" />
      <img id="cloud6" src="img/props/cloud_transparent.png" class="cloud cloud6" />
      
      <img src="img/props/palm_tree.png" class="palm-tree" />
      <div class="text-container" >
        <div class="d-flex justify-content-center">
        <img src="/img/logos/logo1.png" class="logo" />
        </div>
        <div class="d-flex justify-content-center mt-4">
          <label class="montserrat" style="font-size: 22px;"><b>Zero utility, negative value, collectable NFT sharks.</b></label>
        </div>
        <div class="d-flex justify-content-center mt-4">
          <div class="hero-button">
            <a href="https://twitter.com/SharkpunksNFT" style="text-decoration:none;">

              <div class="d-flex justify-content-center px-3">
                <!-- scroll down to how to join -->
                <img class="my-auto" src="/img/logos/twitter_white.png" style="height:24px">
                
                <label class="m-2 open-sans" style="font-size: 20px;color:white">Twitter</label> 
              </div>
            </a>

          </div>
            <div class="hero-button mx-4">
              <a href="https://discord.com/invite/oh-geez" style="text-decoration:none">

                <div class="d-flex justify-content-center px-3">
                  <!-- scroll down to how to join -->
                  <img class="my-auto" src="/img/logos/discord_white.png" style="height:20px">
                  <label class="m-2 open-sans" style="font-size: 20px;color:white">Discord</label> 
                </div>
              </a>

            </div>
        </div>
      </div>

      <div class="ocean-solid ocean-color"  />
    </div>
    <div class="d-flex justify-content-center" style="width:100%;background-color:#F6ECE5;padding-top:120px;padding-bottom:120px">
      <div class="d-flex justify-content-between my-auto" style="width:70%">
        
        <div class="paragraph-container my-auto mx-5" style="text-align:left">
          <p class="montserrat" style="font-size:24px;font-weight:bold">Future utilization of sharkpunks NFTs may include, but are not limited to:</p>
          <br>
          <div class="bullet-point-box py-4 my-3">
          <p class="mx-3 open-sans bullet-points my-auto">Decorative painting in the basement of your mother</p>
          </div>
          <div class="bullet-point-box py-4 my-3">
          <p class="mx-3 open-sans bullet-points my-auto">Comparison of phallus size</p>
          </div>
          <div class="bullet-point-box py-4 my-3">
          <p class="mx-3 open-sans bullet-points my-auto">Companion as you contemplate your existential crisis</p>
          </div>
        </div>
        <div class="mx-5 my-auto">
          <img v-bind:src="shark" style="width:300px"/>
        </div>
      </div>
    </div>
    <br>
    <div style="height:700px">
      <div class="d-flex justify-content-center m-5">
        <h1 class="open-sans"><b>Roadmap</b></h1>
      </div>
      <div style="position:absolute;height:600px;background-color:red" v-bind:style="'left:' + screenCenter + 'px'">
        <div style="position:relative;height:600px">
          <div class="roadmap-bar" style=""/>
          <div class="roadmap-point-checked" style="top:40px" />
          <div class="roadmap-point"  style="top:220px" />
          <div class="roadmap-point" style="top:400px" />
          <div class="roadmap-box"  style="top:0px">
            <div class="d-flex justify-content-center">
              <h2><b>Q4 2021</b></h2>
            </div>
            <label class="montserrat">
              First Sharkpunks minted for LevX Dao genesis members and eligible raffle winners
            </label>
          </div>
          <div class="roadmap-box2" style="top:180px">
            <div class="d-flex justify-content-center">
              <h2><b>Q1 2022</b></h2>
            </div>
            <label class=" montserrat">
              Remaining supply minted up to 10,000 Sharkpunks
            </label>
          </div>
          <div class="roadmap-box"  style="top:360px">
            <div class="d-flex justify-content-center">
              <h2><b>Q1 2022</b></h2>
            </div>
            <label class=" montserrat">
              Sharkpunks listed as one of the first collectibles in shoyu
            </label>
          </div>


          
        </div>
      </div>
    </div>
    <div class="d-flex justify-content-center" v-bind:style="'height:' + (0.7* windowHeight) + 'px'" style="background-color:#F2FEDC">
        <div class="my-auto">
          <h1 class="open-sans" ><b>Join our community</b></h1>
          <div class="d-flex justify-content-center my-5">
            <a href="https://twitter.com/SharkpunksNFT" style="text-decoration:none;">
              <img src="img/logos/twitter.png" class="mx-4" style="width:80px"/>
            </a>
            <a href="https://discord.com/invite/oh-geez" style="text-decoration:none">
              <img src="img/logos/discord.png" class="mx-4" style="width:80px"/>
            </a>
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
  computed : {
    screenCenter: function () {
      return this.windowWidth / 2
    }
  },
  created() {
    window.console.log(this.screenWidth)
    window.console.log(this.windowHeight)
    this.loopImage()
    window.addEventListener('resize', () => {
      this.windowHeight = window.innerHeight
      this.windowWidth = window.outerWidth
    })
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
  unmounted() {
    window.removeEventListener('resize')
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

/* small */

@media only screen and (max-width: 600px) {
  .palm-tree {
    left: 0px;

  }

  .roadmap-box2 {
  position:absolute;
  font-weight:bold;
  font-size:18px;
  width:250px;
  left:100px
  } 
}

  

/* medium */

@media only screen and (min-width: 601px) and (max-width: 1299px){
  .palm-tree {
    left: 150px;
  }
}

/* large */

@media only screen and (min-width: 1300px) {
  .palm-tree {
    left: 100px;
    height: 50%


  }


.palm-tree {
  position:absolute;
    bottom: 0px;
}

  
.roadmap-box2 {
  position:absolute;
  font-weight:bold;
  font-size:18px;
  width:250px;
  right: 70px;
}

.shark {
  position: absolute
}

.shark1 {
  width: 250px;
  right: 50px;
  bottom: -90px;
  
}

.shark2 {
  width: 250px;
  right: 300px;
  bottom: -90px;
  transform: scaleX(-1);

}
.shark3 {
  width: 80px;
  right: 380px;
  bottom: 23%;
  animation-name:shark3-bobble;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}

.shark4 {
  width: 80px;
  right: 470px;
  bottom: 23%;
  animation-name:shark4-bobble;
  animation-duration: 2s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
  animation-delay: 1s;
  transform: scaleX(-1);
}

.shark5 {
  width: 120px;
  right: 600px;
  bottom: 50px;
}

.shark6 {
  width: 120px;
  right: 750px;
  bottom: 50px;
  transform: scaleX(-1)
}

@keyframes shark3-bobble {
  0% {transform: translateY(0%)}
  50% {transform: translateY(-20%)}
}

@keyframes shark4-bobble {
  0% {transform: translateY(0%) scaleX(-1)}
  50% {transform: translateY(-20%) scaleX(-1)}
}




.ocean-solid {
  position:absolute;
  right:350px;
  bottom:23.9%;
  width: 200px;
  height:45px
}

.cloud {
  position:absolute;
}

.cloud1 {
  right: 200px;
  top: 17%;
  width: 100px;
  animation-name:cloud1-animation;
  animation-duration: 45s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}




.cloud2 {
  right: 300px;
  top: 30%;
  width: 200px;
  animation-name:cloud2-animation;
  animation-duration: 30s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}



.cloud3 {
  right: 500px;
  top: 8%;
  width: 300px;
  animation-name:cloud3-animation;
  animation-duration: 15s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}




.cloud4 {
  right: 100px;
  top: 50%;
  width: 50px;
  animation-name:cloud4-animation;
  animation-duration: 60s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}



.cloud5 {
  right: 600px;
  top: 50%;
  width: 60px;
  animation-name:cloud5-animation;
  animation-duration: 55s;
  animation-iteration-count: infinite;
  animation-timing-function:linear;
}




.cloud6 {
  right: 750px;
  top: 50%;
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
  top: 10%;
  left:100px
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
  font-size: 18pxx  

}

.roadmap-bar {
  position:absolute;
  top: 40px;
  width:4px;
  height:360px;
  background-color:black;
  left: -2px;
}

.roadmap-point {
  position:absolute;
  width:20px;
  height:20px;
  border-radius:50%;
  background-color:white;
  left: -10px;
  border-style: solid;
  border-width:3px;
  border-color:black;

} 
.roadmap-point-checked {
  position:absolute;
  width:20px;
  height:20px;
  border-radius:50%;
  background-color:black;
  left: -10px;


} 


.roadmap-box {
  position:absolute;
  font-weight:bold;
  font-size:18px;
  width:250px;
  left: 50px;


}

.bullet-points {
  font-size: 18px;
  color:#8C808F
}

.bullet-point-box {
  background-color:white;
  box-shadow: 0px 0px 5px 2px #c9c1bb;
  border-radius: 5px

}



}



</style>
