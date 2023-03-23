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
    <div>
        <img src="../assets/img/dc-logo.png" alt="dc-logo">
    </div>
       <AppHeaderNav></AppHeaderNav>
  </header>
    
</template>

<style lang="scss" scoped>
@use "../style/variables.scss" as *;
</style>
