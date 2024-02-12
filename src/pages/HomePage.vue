<template>
  <div class="hero-image-container border-bottom border-light border-3">
    <h1 class="d-flex flex-column justify-content-center align-items-center text-center">
      Focus Massage
    </h1>
    <img class=""
      src="https://images.unsplash.com/photo-1574421233376-06f2ccf017f7?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
      alt="">
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 p-md-5 mt-3 align-items-center shadow rounded elevation-3">
      <Services />
    </div>
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 pb-0 p-md-5 pb-md-0 mt-3 align-items-center shadow rounded elevation-3">
      <h2>
        Reviews
      </h2>
      <Reviews />
    </div>
  </div>
  <div class="flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 p-md-5 mt-3 rounded">
      <h2>
        Hours
      </h2>
      <Hours />
    </div>
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 p-md-5 mt-3 rounded">
      <Location />
    </div>
  </div>
  <div class="flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 p-md-5 my-3 align-items-center rounded">
      <About />
    </div>
  </div>
</template>

<script>
import About from "../components/About.vue";
import Hours from "../components/Hours.vue";
import Location from "../components/Location.vue";
import Reviews from "../components/Reviews.vue";
import Services from "../components/Services.vue";


export default {
  setup() {
    return {};
  },
  components: { Reviews, Services, Location, Hours, About }
}
</script >

<style scoped lang="scss">
.hero-image-container {

  img {
    object-position: center 60%;
    object-fit: cover;
    filter: brightness(40%);
    height: 33vh;
    width: 100%;
  }

  h1 {
    position: absolute;
    z-index: 1;
    height: 33vh;
    width: 100%;
    color: antiquewhite;
  }
}

.google-map {
  width: 100%;
  height: 33vh;

}

.home-card {
  min-height: 40vh;
  color: antiquewhite;
  background: rgba(255, 255, 255, 0.2);
  border-radius: 16px;
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  border: 1px solid rgba(255, 255, 255, 0.3);
  text-align: center;
  width: clamp(350px, 70vw, 100%);
}

.home {
  display: grid;
  height: 40vh;
  place-content: center;
  text-align: center;
  user-select: none;
}
</style>
