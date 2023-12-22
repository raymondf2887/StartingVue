<script>
import Rating from "./Rating.vue";

export default {
  props: {
    data: Object,
  },
  components: {
    Rating,
  },
};
</script>
<template>
  <div class="card border-dark mb-3" style="max-width: 1000px; background: linear-gradient(0deg, #ffffff, #32cfff);">
    <div class="card-header" style="color: white; font-size: 30px;">{{ data.productName }}</div>
    <div class="row no-gutters">
      <div class="col-md-4">
        <img :src="data.imageUrl" class="card-img" alt="..." />
      </div>
      <div class="col-md-8">
        <div class="card-body">
          <Rating :initalRating="data.rating" />
          <p class="card-text">{{ data.description }}</p>
          <button type="button" class="btn btn-info">More Info</button>
          <p class="card-text">
            <small class="text-muted">{{ data.releasedDate }}</small>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>