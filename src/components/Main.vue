<template>
  <div>
      <main>
              <div class="main-content">
                  <div class="main-center-top"></div>
                  <div class="main-center-bottom container">

                      <button>Current series</button>

                      <div class="main-box container">
                          <ProdCard 
                          v-for="(element,index) in cards "
                          :key="index"
                          :details="element"
                          />
                      </div>

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
    position: relative;
    }

    .main-center-bottom{
        padding: 80px 15px;
        padding-top:40px;
        overflow: hidden;
        margin-top: 20px;
    }

    .main-center-bottom .main-box{
        display: flex;
        flex-wrap: wrap;
    }

    .main-center-bottom .main-box .card{
        flex-basis: calc(100% / 6 - 20px);
        height: 200px;
        margin: 40px 10px;
        margin-top: 5px;
    }

    button{
        position: absolute;
        bottom: -62px;
        background: #0282f9;
        color: #fff;
        padding: 15px 20px;
        outline: none;
        border: none;
        text-transform: uppercase;
        font-weight: 600;
        font-size:24px ;
    }

</style>