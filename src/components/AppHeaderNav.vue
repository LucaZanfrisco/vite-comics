<script>
export default {
    name: 'AppHeaderNav',
    data(){
        return{
            navList: ['CHARACTERS','COMICS','MOVIES','TV','GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS','SHOP']
        }
    }
}
</script>

<template>
    <!-- Nav Bar -->
    <nav>
        <ul>
            <li v-for="nav in navList">{{ nav }}</li>
        </ul>
    </nav>
    <!-- /Nav Bar -->
</template>

<style lang="scss" scoped>
@use "../style/variables.scss" as *;
// Stile della nav
nav{
    padding: 0 1.25rem;
    height: 100%;
    line-height: 7.5rem;
    ul{
        display: flex;
        height: 100%;
        li{
            padding: 0 1.0625rem;
            font-weight: bold;
            &:hover{
                cursor: pointer;
                color: $primary-color;
                border-bottom: 3px solid $primary-color;
            }
        }
    }
}
</style>