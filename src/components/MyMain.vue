<template>

  <main>
      <section class="">
          <div class="container">
              <MyList />
          </div>
      </section>
  </main>
  
</template>

<script>
import MyList from './MyList.vue'

export default {
    components:{
        MyList,
    }
    
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

main {
    background-color: #1e2d3b;
    min-height:100vh;
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

</style>