<template>
  <h2>
    Location
  </h2>
  <iframe
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2890.435316719675!2d-116.56382762434703!3d43.57664825737948!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x54ae4d164cfb8781%3A0xaf91dccc44109896!2sFocus%20Massage!5e0!3m2!1sen!2sus!4v1707233805753!5m2!1sen!2sus"
    class="google-map rounded mt-3" allowfullscreen="" loading="lazy"
    referrerpolicy="no-referrer-when-downgrade"></iframe>
</template>


<script>
export default {
  setup() {
    return {}
  }
}
</script>


<style lang="scss" scoped>
.google-map {
  width: 100%;
  height: 33vh;

}
</style>