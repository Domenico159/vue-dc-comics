<template>
      <footer>
          <div class="container">
              <div class="box-links">
                  <ul>
                      <li>
                          <h3>dc comics</h3>
                          <a href="">characters</a>
                          <a href="">comics</a>
                          <a href="">movies</a>
                          <a href="">tv</a>
                          <a href="">games</a>
                          <a href="">videos</a>
                          <a href="">news</a>
                      </li>
                       <li>
                           <h3>dc</h3>
                          <a href="">terms of use</a>
                          <a href="">privacy policy (new)</a>
                          <a href="">ad choises</a>
                          <a href="">advertising</a>
                          <a href="">jobs</a>
                          <a href="">subscriptions</a>
                          <a href="">talent workshops</a>
                          <a href="">CPSC Certificates</a>
                          <a href="">ratings</a>
                          <a href="">shop help</a>
                          <a href="">contact us</a>
                      </li>
                       <li>
                           <h3>sites</h3>
                          <a href="">DC</a>
                          <a href="">MAD Magazine</a>
                          <a href="">Dc Kids</a>
                          <a href="">DC universe</a>
                          <a href="">Dc Power Visa</a>
                      </li>
                       <li>
                           <h3>Shop</h3>
                          <a href="">Shop DC</a>
                          <a href="">Shop DC collectibles</a>
                      </li>
                  </ul>
              </div>

              <div class="box-img">
              <img src="../assets/img/dc-logo-bg.png" alt="">
             </div>
          </div>
          <div class="footer-bottoom">
              <div class="container">
                  <div class="btn">
                      <button>Sing-up now!</button>
                  </div>
                  <div class="follow">
                      <ul>
                          <li>
                              <a href=""><h2>follow us</h2></a>
                          </li>
                          <li>
                              <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
                          </li>
                          <li>
                              <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
                          </li>
                          <li>
                              <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
                          </li>
                          <li>
                              <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
                          </li>
                          <li>
                              <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
                          </li>
                      </ul>
                  </div>
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
    background-size:cover ;
    position: relative;
    overflow: hidden;
}

footer .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}


footer .container .box-img{
    overflow: hidden;
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
    display: flex;
    flex-direction: column;
}

footer .container .box-links ul li h3{
    text-transform: uppercase;
    margin-bottom: 15px;
}



footer .container .box-links ul li a,
footer .container .box-links ul li h3{
    color: #fff;
}

footer .container .box-links ul li a{
    font-size:12px ;
    color: #6b6f7d;
    text-transform: capitalize;
    margin-top:5px ;
}

footer .container .box-links ul li a:hover{
    color: #1e90ff;
}

footer .footer-bottoom{
    background: #303030;
}

footer .footer-bottoom .container{
   height: 100px;
}

footer .footer-bottoom .container .follow ul {
    list-style: none;
    display: flex;
}

footer .footer-bottoom .container .follow ul li{
    margin-right:15px ;
}

footer .footer-bottoom .container .btn button{
    width: 150px;
    height: 50px;
    background: none;
    text-transform: uppercase;
    color: #fff;
    font-size: 18px;
    border: 2px solid #1e90ff;

}

footer .footer-bottoom .container .follow ul li a h2{
    text-transform: uppercase;
    color: #1e90ff;
}

</style>