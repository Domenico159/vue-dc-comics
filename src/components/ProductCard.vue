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

.main-center-bottom .main-box .card{
        flex-basis: calc(100% / 6 - 40px);
        margin: 15px 18px;
        transition: transform 0.3s;
        cursor: pointer;
    }

    .main-center-bottom .main-box .card:hover{
        transform: scale(1.1);
    }

    .main-center-bottom .main-box .card h3{
        text-transform: uppercase;
        font-size: 12px;
        color: #b9bbb2;
    }


.card .box-img{
    width: 100%;
    margin-bottom: 10px;
}

</style>