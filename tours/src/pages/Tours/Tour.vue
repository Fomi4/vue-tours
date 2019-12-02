<template lang="html">
  <div>
    <img :src="img" :alt="description" width="150">
    <p>Destination: {{ destination }}</p>
    <p>Date: {{ date }}</p>
    <p>Description: {{ description }}</p>
  </div>
</template>

<script>
export default {
  name: 'Tour',
  props: {
    destination: {
      default: 'Unknown',
      type: String
    },
    date: Number,
    img: {
      default: 'https://classifieds.recordcourier.com/public/images/no-photo.png',
      type: String
    },
    description: {
      default: 'Unknown',
      type: String
    }
  }
}
</script>

<style lang="css" scoped>
</style>