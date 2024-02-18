<template>
  <div class="hero-image-container ">
    <h1 class="d-flex flex-column justify-content-center align-items-center text-center">
      Focus Massage
    </h1>
    <img
      src="https://images.unsplash.com/photo-1574421233376-06f2ccf017f7?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
      alt="Focus Massage Hero Image">
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 p-md-5 mt-3 align-items-center rounded">
      <Services />
    </div>
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 pb-0 p-md-5 pb-md-0 mt-3 align-items-center rounded">
      <Reviews />
    </div>
  </div>
  <div class="flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-4 p-md-5 mt-3 rounded">
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
      Meet the therapist
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
  border-bottom: 4px var(--text-main) solid;

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
    color: var(--text-main);
    font-weight: bold;
    text-shadow: rgb(0, 0, 0) 1px 10px 10px;
  }
}

.home-card {
  // min-height: 40vh;
  color: var(--text-main);
  text-align: center;
  width: clamp(350px, 70vw, 100%);
}

.glassmorphism {
  background: rgba(255, 255, 255, 0.2);
  border-radius: 16px;
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  border: 1px solid rgba(255, 255, 255, 0.3);
}

.home {
  display: grid;
  height: 40vh;
  place-content: center;
  text-align: center;
  user-select: none;
}
</style>
