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
import '..//assets/scss/_common.scss';


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
    align-items: center;
    justify-content: center;
    padding:90px 20px;

}

</style>