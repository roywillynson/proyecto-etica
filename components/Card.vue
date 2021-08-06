<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="url" alt="Card image" class="p-6">
      </figure>
    </div>
    <div class="card-content">

      <p class="content has-text-centered is-size-4">
        {{ text }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true
    },
    url: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.card {
  border-radius: 20px;
  overflow: hidden;
  transition: 0.4s transform ease;

  &:hover {
    border-color: white;
    transform: scale(1.1);
    transform-origin: center;
  }
}
</style>
