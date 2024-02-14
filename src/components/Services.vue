<template>
  <h2 class="mb-3">
    Services
  </h2>
  <section class="row">
    <div class="col-12 col-md-4 m-auto" v-for="service in  services " :key="service.id">
      <ServiceCard :service="service" />
    </div>
  </section>
  <section class="row d-flex d-md-none ">
    <BookNow />
  </section>
</template>


<script>

import { SERVICES_TYPES } from "../constants";
import BookNow from "./BookNow.vue";

export default {
  setup() {
    const services = SERVICES_TYPES;
    return {
      services
    };
  },
  components: { BookNow }
}
</script>


<style lang="scss" scoped></style>