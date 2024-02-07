<template>
  <div v-for="service in  services " :key="service.id">
    <ServiceCard :service="service" />
  </div>
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