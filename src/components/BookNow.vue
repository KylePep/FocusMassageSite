<template>
  <a class="d-flex justify-content-center" href="https://danawhalen.glossgenius.com/services">
    <button class="btn nav-button d-flex fw-bold py-3 px-5 ms-2 rounded">
      Book Now!
    </button>
  </a>
</template>


<script>
export default {
  setup() {
    return {}
  }
}
</script>


<style lang="scss" scoped>
.nav-button {
  color: var(--text-main);
  pointer-events: auto;
  background-color: rgba(128, 128, 128, 0.491);
}

.nav-button:hover {
  color: whitesmoke;
  background-color: gray;
}
</style>