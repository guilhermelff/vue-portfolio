<template>
  <div>
    <section class="showcase">
      <header>
        <h2 class="logo">LOGO AQUI</h2>
        <div class="toggle"></div>
      </header>

      <video
        type="video/mp4"
        src="../src/assets/video-fundo-est3.mp4"
        muted
        loop
        autoplay
      ></video>

      <div class="text">
        <h2>Never Stop</h2>
        <h3>Exploring The World</h3>
        <p>
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptatem
          provident accusamus explicabo, minus tempora expedita numquam quo
          fugit autem veniam!
        </p>
        <a href="#">Explore</a>
      </div>

      <ul class="social">
        <li>linkedin</li>
        <li>github</li>
      </ul>
    </section>

    <div class="menu">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Home</a></li>
        <li><a href="#">Home</a></li>
        <li><a href="#">Home</a></li>
        <li><a href="#">Home</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  setup() {},
};
</script>

<style>
#app {
  font-family: "regular", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

@font-face {
  font-family: "light";
  src: url("../src/assets/fontes/Ubuntu-Light.ttf");
}

@font-face {
  font-family: "regular";
  src: url("../src/assets/fontes/Ubuntu-Regular.ttf");
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.showcase {
  position: absolute;
  right: 0;
  width: 100%;
  min-height: 100vh;
  padding: 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #111;
  color: #fff;
  z-index: 2;
}

.showcase header {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  padding: 40px 100px;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
}

.toggle {
  position: relative;
  width: 60px;
  height: 60px;
  background: url("../src/assets/hamburguer.png");
  background-repeat: no-repeat;
  background-size: 30px;
  background-position: center;
  cursor: pointer;
}

.toggle.active {
  background: url("../src/assets/close.png");
  background-repeat: no-repeat;
  background-size: 25px;
  background-position: center;
}

.showcase video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  opacity: 0.8;
}

.text {
  position: relative;
  z-index: 10;
}
</style>
