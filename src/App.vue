<template>
  <div id="app">
    <div class="container">
      <h1>Who do you want to marry in Sword Art Online?</h1>
      <div id="myCarousel" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class></li>
          <li data-target="#myCarousel" data-slide-to="1" class="active"></li>
          <li data-target="#myCarousel" data-slide-to="2" class></li>
        </ol>
        <div class="carousel-inner">
          <div class="carousel-item">
            <img :src="img[3].src" class="img-fluid" style=" border-radius: 8px; width: 1280px; hight: 720px;" />
          </div>
          <div class="carousel-item active">
            <img :src="img[4].src" class="img-fluid" style=" border-radius: 8px; width: 1280px; hight: 720px;"/>
          </div>
          <div class="carousel-item">
            <img :src="img[5].src" class="img-fluid" style=" border-radius: 8px; width: 1280px; hight: 720px;"/>
          </div>
          <a class="carousel-control-prev" href="#myCarousel" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a class="carousel-control-next" href="#myCarousel" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>
    </div>
    <div class="container">
      <hr class="featurette-divider" />
      <div class="row featurette alert alert-info" style="opacity: 0.9; border-radius: 8px; ">
        <div class="row align-items-center">
          <div class="col-6">
            <!-- 2.รับค่าจาก emit @cc แล้วส่งไปทำงานใน function "sum"-->
            <h3>Yuuki Asuna</h3>
            <like label @cc="sum" />
          </div>
          <div class="col-6">
            <img :src="img[0].src" class="img-fluid" />
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <hr class="featurette-divider" />
      <div class="row featurette alert alert-info" style="opacity: 0.9; border-radius: 8px; ">
        <div class="row align-items-center">
          <div class="col-6">
            <img :src="img[1].src" class="img-fluid" />
          </div>
          <div class="col-6">
            <!-- 2.รับค่าจาก emit @cc แล้วส่งไปทำงานใน function "sum"-->
            <h3>Alice Zuberg</h3>
            <like label @cc="sum" />
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <hr class="featurette-divider" />
      <div class="row featurette alert alert-info" style="opacity: 0.9; border-radius: 8px; ">
        <div class="row align-items-center">
          <div class="col-6">
            <!-- 2.รับค่าจาก emit @cc แล้วส่งไปทำงานใน function "sum"-->
            <h3>Asada Shino</h3>
            <like label @cc="sum" />
          </div>
          <div class="col-6">
            <img :src="img[2].src" class="img-fluid" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Like from "./components/Like.vue";

export default {
  name: "App",
  components: { Like },
  data: function () {
    return {
      img: [
        {
          src:"https://i.pinimg.com/originals/42/8f/90/428f90ce15242ec6dd33565ac4887ccf.jpg"
        },
        {
          src:
            "https://wallpapercave.com/wp/wp5183417.jpg",
        },
        {
          src:
            "https://www.teahub.io/photos/full/251-2512720_sinon-sao-wallpaper-4k..png",
        },
        {
          src:
            "https://images7.alphacoders.com/834/834502.jpg",
        },
        {
          src:
            "https://images5.alphacoders.com/700/700049.jpg",
        },
        {
          src:
            "https://wallpapercave.com/wp/wp2458414.pngn",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: 'Annie Use Your Telescope', cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000000;
  margin-top: 60px;
}
body {
  background-image: url("./assets/bg.jpg");
  background-repeat: no-repeat;
  background-attachment: fixed; 
  background-size: 100% 100%;
}
</style>
