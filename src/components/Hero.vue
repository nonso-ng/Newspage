<template>
  <div class="hero">
    <div class="hero-left">
      <div class="hero-left-top"></div>
      <div class="hero-left-top-mobile"></div>
      <div class="hero-left-bottom">
        <div class="hero-left-bottom-left">
          <h1>The Bright Future Of Web 3.0?</h1>
        </div>

        <div class="hero-left-bottom-right">
          <p>
            We dive into the next evolution of the web that claims to put the
            hplatforms back into the hands of the people. But is it really
            fulfilling its promise?
          </p>
          <button class="btn">READ MORE</button>
        </div>
      </div>
    </div>
    <div class="hero-right">
      <h1 style="color: hsl(35, 77%, 62%)">New</h1>
      <h3>{{ news[0].title }}</h3>
      <p>Will hydrogen fueled cars ever actch up to EVs?</p>
      <hr />

      <h3>{{ news[1].title }}</h3>
      <p>{{ news[1].paragraph }}</p>
      <hr />

      <h3>{{ news[2].title }}</h3>
      <p>{{ news[2].paragraph }}</p>
    </div>
  </div>
</template>

<style scoped>
.hero {
  background-color: white;
  display: grid;
  gap: 15px;
  height: 70vh;
  grid-template-columns: 2.1fr 0.9fr;
  font-family: "Inter", sans-serif;
}

.hero-right {
  background-color: hsl(240, 100%, 5%);
  color: white;
  padding: 10%;
  height: 55vh;
}
.hero-right p {
  font-size: medium;
  font-weight: 100;
  color: gray;
}
.hero-left-top {
  background-image: url(../assets/image-web-3-desktop.jpg);
  background-size: cover;
  height: 40vh;
}

.hero-left-bottom {
  display: grid;
  grid-auto-flow: column;
  grid-template-columns: 0.9fr 1.1fr;
  gap: 15px;
  height: 25vh;
  margin-top: 15px;
  padding-top: 15px;
}

.hero-left-bottom-left h1 {
  margin-top: -5px;
  font-size: 47px;
  font-weight: 900;
}
.hero-left-bottom-right {
  display: flex;
  flex-direction: column;
  color: gray;
  font-size: 15px;
  padding-left: 40px;
  padding-right: 20px;
}

.btn {
  background-color: hsl(5, 85%, 63%);
  color: white;
  border-style: none;
  width: 180px;
  letter-spacing: 4px;
  padding: 15px;
  margin-top: 15px;
}
.btn:hover {
  background-color: hsl(240, 100%, 5%);
}

@media (max-width: 800px) {
  .hero {
    display: flex;
    flex-direction: column;
    height: 100%;
  }
  .hero-left-top {
    display: none;
    /* 
     */
  }
  .hero-left-top-mobile {
    display: flex;
    background-image: url(../assets/image-web-3-mobile.jpg);
    background-size: cover;
    height: 55vh;
    margin: auto 3%;
  }

  .hero-left-bottom {
    display: flex;
    flex-direction: column;
    height: 60vh;
  }

  .hero-left-bottom-left h1 {
    margin: auto 3%;
  }

  .hero-left-bottom-right {
    padding: 0;
    margin:0% 3% 0% 3%;
  }

  .hero-left-bottom-right p{
    line-height: 2.3;
  }
.hero-right{
  margin: auto 3%;
}
.hero-right {
height: 60%;
}


}
</style>

<script setup>
let news = [
  {
    title: "Hydrogen VS Electric Cars",
    paragraph: "Will hydrogen fueled cars ever actch up to EVs?",
  },
  {
    title: "The Downsides of AI artistry",
    paragraph:
      "What are the possible on demand effect of on-demand AI image generation?",
  },
  {
    title: "Is VC funding drying up?",
    paragraph:
      "Private funding by VC firms is down 50% YOY, Wtake a look at what that means",
  },
];
</script>
