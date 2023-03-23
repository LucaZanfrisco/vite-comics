<script>
    export default{
        name: 'AppMain'
    }
</script>

<template>
    <main>
        <div class="products">
            -- Content Goes Here --
        </div>
    </main>
    
</template>

<style lang="scss" scoped>
    @use '../style/variables.scss' as *; 

    main{
        background-color: black;
        height: 8.4375rem;
        .products{
            @include container;
            height: 100%;
            color: white;
            display: flex;
            align-items: center;
            font-size: 1.5rem;
    } 
    }
   
</style>