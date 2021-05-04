<template>
      <footer>
          <div class="container">
              <div class="box-links">
                  <ul>
                      <li>
                          <h3>Titolo</h3>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                      </li>
                       <li>
                           <h3>Titolo</h3>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                      </li>
                       <li>
                           <h3>Titolo</h3>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                      </li>
                       <li>
                           <h3>Titolo</h3>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                          <a href=""></a>
                      </li>
                  </ul>
              </div>

              <div class="box-img">
              <img src="../assets/img/dc-logo-bg.png" alt="">
             </div>

          </div>
      </footer>
</template>

<script>
export default {
    name:'Footer',
}
</script>

<style scoped>

footer{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 500px;
    position: relative;
    overflow: hidden;
}

footer .container{
    display: flex;
    justify-content: space-between;
}

footer .container .box-links{
    padding: 30px 10px;
}

footer .container .box-links ul {
    display: flex;
    flex-wrap: wrap;
    list-style: none;
}

footer .container .box-links ul li{
    flex-basis: calc(100% / 3 - 15px);
    margin: 7px;
}

footer .container .box-links ul li a,
footer .container .box-links ul li h3{
    color: #fff;
}

</style>