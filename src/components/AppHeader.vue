<script>
import AppHeaderNav from './AppHeaderNav.vue';
export default {
  name: 'AppHeader',
  components:{
    AppHeaderNav,
  }
}
</script>

<template>
  <header>
    <!-- Contenitore Logo -->
    <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="dc-logo">
    </div>
    <!-- Componente NavBar Header -->
       <AppHeaderNav></AppHeaderNav>
  </header>
    
</template>

<style lang="scss" scoped>
@use "../style/variables.scss" as *;

header{
    @include container;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 7.5rem;
    .logo{
        max-width: 5rem;
        max-height: 5rem;
        img{
            width: 100%;
        }
    }
}
</style>
