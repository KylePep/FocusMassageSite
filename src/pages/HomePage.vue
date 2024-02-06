<template>
  <div class="hero-image-container">
    <h1 class="d-flex flex-column justify-content-center align-items-center text-center text-light">
      Focus Massage
    </h1>
    <img class=""
      src="https://images.unsplash.com/photo-1574421233376-06f2ccf017f7?q=80&w=2069&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
      alt="">
  </div>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 card align-items-center shadow rounded elevation-3">
      <h2>
        Location
      </h2>
    </div>
  </div>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 card align-items-center shadow rounded elevation-3">
      <h2>
        Hours
      </h2>
    </div>
  </div>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 card align-items-center shadow rounded elevation-3">
      <h2>
        Services
      </h2>
    </div>
  </div>
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 card align-items-center shadow rounded elevation-3">
      <h2>
        Stuff
      </h2>
      <h2>
        Things
      </h2>
    </div>
  </div>
</template>

<script>
export default {
  setup() {
    return {

    }
  }
}
</script>

<style scoped lang="scss">
.hero-image-container {
  position: relative;

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
  }
}


.home {
  display: grid;
  height: 40vh;
  place-content: center;
  text-align: center;
  user-select: none;

  .home-card {
    width: clamp(350px, 50vw, 100%);
  }
}
</style>
