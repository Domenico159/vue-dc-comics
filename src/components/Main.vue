<template>
  <div>
      <main>
              <div class="main-content">
                  <div class="main-center-top"></div>
                  <div class="main-center-bottom container">

                      <button class="btn1">Current series</button>

                      <div class="main-box container">
                          <ProdCard 
                          v-for="(element,index) in cards "
                          :key="index"
                          :details="element"
                          />
                      </div>
                  </div>
                  <div class="btn-buttom container">
                          <button class="btn2">Load more</button>
                      </div>
              </div>
              <div class="main-bottom">
                  <ul class="container">
                      <li>
                          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                          <a href="">digital comics</a>
                      </li>
                      <li>
                          <img src="../assets/img/buy-comics-merchandise.png" alt="">
                          <a href="">dc merchandise</a>
                      </li>
                      <li>
                          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                          <a href="">subscriptions</a>
                      </li>
                      <li>
                          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                          <a href="">comic shop locator</a>
                      </li>
                      <li>
                          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                          <a href="">dc power visa</a>
                      </li>
                  </ul>
              </div>
      </main>
  </div>
</template>

<script>
import ProdCard from '@/components/ProductCard.vue';
import cards from '@/data/cards.js';

export default {
    name:'Main',
    components:{
        ProdCard,
    },
    data(){
        return {
            cards:cards,
        }
    }
}
</script>

<style scoped>

main{
    background: #1c1c1c;
    color: #fff;
}


.main-bottom{
    background: #1e90ff;
}

.main-bottom ul {
    display: flex;
    list-style: none;
    padding: 40px 10px;
}
.main-bottom ul li{
    display: flex;
    align-items: center;
    flex-basis: calc(100% / 5 - 10px);
}
.main-bottom ul li a {
    color: #fff;
    margin-left: 30px;
    text-transform: uppercase;
    font-size: 14px;
}
.main-bottom ul li img{
    width: 50px;
}

/* main center */
.main-center-top{
    height: 500px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    }

    .main-center-bottom{
        padding-top:40px;
        margin-top: 20px;
        padding-bottom: 30px;
        position: relative;
    }

    .main-center-bottom .main-box{
        display: flex;
        flex-wrap: wrap;
    }

    
    button.btn1{
        position: absolute;
        top: -48px;
        background: #0282f9;
        color: #fff;
        padding: 15px 20px;
        outline: none;
        border: none;
        text-transform: uppercase;
        font-weight: 600;
        font-size:24px ;
    }

    .btn-buttom{
        display: flex;
        justify-content: center;
    }

    .btn-buttom button.btn2{
        background: #0282f9;
        color: #fff;
        padding: 10px 40px;
        outline: none;
        border: none;
        text-transform: uppercase;
        font-weight: 600;
        font-size:16px ;
        margin-bottom: 20px;
    }

</style>