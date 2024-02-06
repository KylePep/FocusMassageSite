<template>
  <img class="hero-image"
    src="https://images.unsplash.com/photo-1620733723572-11c53f73a416?q=80&w=1887&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
    alt="">
  <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 card align-items-center shadow rounded elevation-3">
      <h1 class="my-5 bg-dark text-white p-3 rounded text-center">
        Focus Massage
      </h1>
    </div>
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
.hero-image {
  object-position: center center;
  object-fit: cover;
  height: 30vh;
  width: 100%;
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
