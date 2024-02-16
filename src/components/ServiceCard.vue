<template>
  <section class="row service-card bg-light text-dark mx-1 my-2">
    <div class="col-12 p-0">
      <img class="ClassicService_image__n_zT4 img-fluid" :src="props.service.image" alt="60 Minute Massage">
    </div>
    <div class="col-12 d-flex flex-column justify-content-between p-3">
      <div>
        {{ service.name }}
        <p class="mt-2">
          {{ service.description }}
        </p>
      </div>
      <div class="text-end">{{ service.price }} | {{ service.duration }} minutes</div>
    </div>
  </section>
</template>


<script>
export default {
  props: {
    service: {
      type: Object,
      required: true
    }
  },
  setup(props) {
    return {
      props
    }
  }
}
</script>


<style lang="scss" scoped>
.service-card {
  border-radius: 2px;
  min-height: 70vh;

  img {
    border-radius: 2px;
  }
}
</style>