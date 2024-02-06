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
    <div class="home-card p-5 mt-3 align-items-center shadow rounded elevation-3">
      <h2>
        Services
      </h2>
    </div>
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 mt-3 align-items-center shadow rounded elevation-3">
      <h2>
        Reviews
      </h2>
    </div>
  </div>
  <div class="flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 mt-3 rounded">
      <h2>
        Hours
      </h2>
      <table class="d-flex justify-content-center mt-3">
        <tr>
          <th>Sunday</th>
          <td>Closed</td>
        </tr>
        <tr>
          <th>Monday</th>
          <td>Closed</td>
        </tr>
        <tr>
          <th>Tuesday</th>
          <td>11am - 6pm</td>
        </tr>
        <tr>
          <th>Wednesday</th>
          <td>8am - 1pm</td>
        </tr>
        <tr>
          <th>Thursday</th>
          <td>11am - 6pm</td>
        </tr>
        <tr>
          <th>Friday</th>
          <td>8am - 3pm</td>
        </tr>
        <tr>
          <th>Saturday</th>
          <td>Closed</td>
        </tr>
      </table>
    </div>
  </div>
  <div class=" flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 mt-3 rounded">
      <h2>
        Location
      </h2>
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2890.435316719675!2d-116.56382762434703!3d43.57664825737948!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x54ae4d164cfb8781%3A0xaf91dccc44109896!2sFocus%20Massage!5e0!3m2!1sen!2sus!4v1707233805753!5m2!1sen!2sus"
        class="google-map rounded mt-3" allowfullscreen="" loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"></iframe>
    </div>
  </div>
  <div class="flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 mt-3 align-items-center shadow rounded elevation-3">
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

table {
  border-spacing: 20px;
}

th,
td {
  padding-left: 20px;
  padding-right: 20px;
}

th {
  text-align: left;
}

td {
  text-align: right;
}
</style>
