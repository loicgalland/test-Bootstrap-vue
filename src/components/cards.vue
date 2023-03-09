<template>
  <div class="card p-0" style="width: 18rem;">
    <img :src="image" :alt="image" class="card-img-top">
    <div class="card-body">
      <h5 class="card-title">{{ title }}</h5>
      <p class="card-text">{{ description }}</p>
      <button class="btn btn-primary"> En savoir plus</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardsHotels',
  props:["title", "description", "id", "image"]
}
</script>

<style scoped lang="scss">
.card{
  margin:10px 10px 0px 10px;
}
</style>
