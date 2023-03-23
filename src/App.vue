<script>
    import AppHeader from './components/AppHeader.vue';
    import AppMain from './components/AppMain.vue';
    import AppFooter from './components/AppFooter.vue';
    export default{
        components:{
            AppHeader,
            AppMain,
            AppFooter
        }
    }
</script>

<template>
    <!-- Componente Header -->
    <AppHeader></AppHeader>
    <!-- Componente Main -->
    <AppMain></AppMain>
    <!-- Componente Main -->
    <AppFooter></AppFooter>
</template>

<style lang="scss">
@use "./style/variables.scss" as *;
li{
    list-style: none;
}

</style>
