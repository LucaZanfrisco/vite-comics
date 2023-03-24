<script>
export default {
    name: 'AppHeaderNav',
    data(){
        return{
            navList: [
                {
                    name: 'CHARACTERS',
                    active: true
                },
                {
                    name: 'COMICS',
                    active: false
                },
                {
                    name: 'MOVIES',
                    active: false
                },
                {
                    name: 'TV',
                    active: false
                },
                {
                    name: 'GAMES',
                    active: false
                },
                {
                    name: 'COLLECTIBLES',
                    active: false
                },
                {
                    name: 'VIDEOS',
                    active: false
                },
                {
                    name: 'FANS',
                    active: false
                },
                {
                    name: 'NEWS',
                    active: false
                },
                {
                    name: 'SHOP',
                    active: false
                }
            ]
        }
    },
    methods:{
        isActive(index){
            this.navList.forEach((element,i) => {
                if(index === i){
                    element.active = true;
                }else{
                    element.active = false;
                }
            })
        }
    }
}
</script>

<template>
    <!-- Nav Bar -->
    <nav>
        <ul>
            <li v-for="(nav,index) in navList" @click="isActive(index)" :class="{active: nav.active}">{{ nav.name }}</li>
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
            }
        }
    }
    .active{
        color: $primary-color;
        border-bottom: 5px solid $primary-color;
    }
}
</style>