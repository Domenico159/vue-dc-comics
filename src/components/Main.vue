<template>
  <div>
      <main>
              <div class="main-content container">
                  <h2> Content goes here </h2>
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
export default {
    name:'Main',
}
</script>

<style scoped>

main{
    background: #1c1c1c;
    color: #fff;
}

.main-content{
    height: 100px;
    display: flex;
    align-items: center;
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

</style>