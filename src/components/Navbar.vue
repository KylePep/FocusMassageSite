<template>
  <div class="navbar d-none d-md-flex position-absolute">
    <a class="" href="https://danawhalen.glossgenius.com/services">
      <button class="btn nav-button d-flex align-items-center text-light fw-bold py-3 px-5 ms-2 rounded">
        Book Now
      </button>
    </a>
  </div>
</template>

<script>
import { onMounted, ref } from 'vue';
import { loadState, saveState } from '../utils/Store.js';
import Login from './Login.vue';
export default {
  setup() {

    const theme = ref(loadState('theme') || 'light')

    onMounted(() => {
      document.documentElement.setAttribute('data-bs-theme', theme.value)
    })

    return {
      theme,
      toggleTheme() {
        theme.value = theme.value == 'light' ? 'dark' : 'light'
        document.documentElement.setAttribute('data-bs-theme', theme.value)
        saveState('theme', theme.value)
      }
    }
  },
  components: { Login }
}
</script>

<style scoped>
.navbar {
  width: 100%;
  height: 33vh;
  pointer-events: none;
}

.nav-button {
  pointer-events: auto;
  background-color: rgba(128, 128, 128, 0.491);
}

.nav-button:hover {
  background-color: gray;
}
</style>
