<script>
export default {
    name: 'AppHeaderNav',
}
</script>

<template>
    <!-- Nav Bar -->
    <nav>
        <ul>
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
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