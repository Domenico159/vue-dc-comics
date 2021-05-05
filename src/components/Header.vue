<template>
  <div>
      <header>
          <nav class="container">
              <a href=""><img src="../assets/img/dc-logo.png" alt=""></a>
              <ul>
                  <li v-for="(element,index) in links" :key="index">
                      <a :href="element.url">{{ element.name }}</a>
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
    data(){

        return {
            links:[
                {
                name:'characters',
                url:'#'
            },
            {
                name:'comics',
                url:'#'
            },
            {
                name:'movies',
                url:'#'
            },
            {
                name:'tv',
                url:'#'
            },
            {
                name:'games',
                url:'#'
            },
            {
                name:'collectibles',
                url:'#'
            },
            {
                name:'videos',
                url:'#'
            },
            {
                name:'fans',
                url:'#'
            },
            {
                name:'news',
                url:'#'
            },
            {
                name:'shop',
                url:'#'
            },
            ]
        }

    },
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
    bottom: -45px;
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