<template>
  <h2 class="mb-3">
    Services
  </h2>
  <section class="row">
    <div class="col-4 m-auto" v-for="service in  services " :key="service.id">
      <ServiceCard :service="service" />
    </div>
  </section>
</template>


<script>

import { SERVICES_TYPES } from "../constants";

export default {
  setup() {
    const services = SERVICES_TYPES
    return {
      services
    }
  }
}
</script>


<style lang="scss" scoped></style>