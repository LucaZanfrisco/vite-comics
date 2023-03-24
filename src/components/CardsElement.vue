<script>
export default {
    name: 'Cards',
    props:{
        image: String,
        name: String,
    }
}
</script>

<template>
    <div >
        <div><img :src="image" :alt="name"></div>
        <div class="title">{{ name }}</div>
    </div>
</template>