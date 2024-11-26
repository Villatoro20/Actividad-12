<template>
  <div class="col-md-4 col-sm-6 col-12 mb-4">
    <div class="card">
      <img :src="iconUrl" class="card-img-top" alt="Chuck Norris Icon">
      <div class="card-body">
        <p class="card-text">{{ value }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    iconUrl: {
      type: String,
      required: true,
    },
    value: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.card {
  border: 1px solid #ccc;
  border-radius: 5px;
}
.card-img-top {
  max-height: 150px;
  object-fit: contain;
  padding: 10px;
}
.card-text {
  font-size: 1rem;
  text-align: justify;
}
</style>
