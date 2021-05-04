<template>
  <div>
      <main>
              <div class="main-content container">
                  <h2> Content goes here </h2>
              </div>
              <div class="main-bottom">

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
</style>