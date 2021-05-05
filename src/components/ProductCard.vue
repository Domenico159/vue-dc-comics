<template>
  <div class="card">
       <div class="box-img">
          <img :src="details.thumb" alt="">
       </div>
      <h3>{{ details.series }}</h3>
  </div>
</template>

<script>
export default {
    name:'ProdCard',
    props:['details']
}
</script>

<style scoped>

img {
    width: 100%;
    object-fit: cover;
}

.card .box-img{
    width: 130px;
    margin-bottom: 15px;
}

</style>