<template>
  <div>
      <header>
          <nav class="container">
              <a href=""><img src="../assets/img/dc-logo.png" alt=""></a>
              <ul>
                  <li>
                      <a href="">characters</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">comics</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">movies</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">tv</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">games</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">collectibles</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">videos</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">fans</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">news</a>
                      <div class="bar"></div>
                  </li>
                  <li>
                      <a href="">shop</a>
                      <div class="bar"></div>
                  </li>
              </ul>
          </nav>
      </header>
  </div>
</template>

<script>
export default {
    name:'Header',
}
</script>

<style scoped>

header nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}

header nav img{
    width: 65px;
}

header nav ul {
    display: flex;
    list-style: none;
}

header nav ul li {
    margin-right: 15px;
    text-transform: uppercase;
    font-size: 16px;
    font-weight: 600;
    position: relative;
}

header nav ul li .bar{
    position: absolute;
    bottom: -50px;
    height: 5px;
    width: 100%;
    background: dodgerblue;
    visibility: hidden;
}

header nav ul li:hover a{
    color: dodgerblue;
}

header nav ul li:hover .bar{
    visibility: visible;
    
}

</style>