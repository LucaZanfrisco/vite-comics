<script>
export default {
    name: 'AppFooterBottom',
    data(){
        return{
            socialList: [
                {
                    image: 'src/assets/img/footer-facebook.png',
                    name: 'button-facebook'
                },
                {
                    image: 'src/assets/img/footer-twitter.png',
                    name: 'button-twitter'
                },
                {
                    image: 'src/assets/img/footer-youtube.png',
                    name: 'button-youtube'
                },
                {
                    image: 'src/assets/img/footer-pinterest.png',
                    name: 'button-pinterest'
                },
                {
                    image: 'src/assets/img/footer-periscope.png',
                    name: 'button-periscope'
                }
            ]
        }
    }
}
</script>

<template>
    <!-- Contenitore della parte inferiore del footer -->
    <div class="footer-bottom-container">
        <!-- Bottone di iscrizione -->
        <div>
            <button>SIGN-UP NOW!</button>
        </div>
        <!-- Lista dei social -->
        <div>
            <ul>
                <li class="follow">FOLLOW US</li>
                <li v-for="social in socialList">
                    <img :src="social.image" :alt="social.name">
                </li>
            </ul>
        </div>
        <!-- /Lista dei social -->
    </div>
</template>

<style lang="scss" scoped>
@use "../style/variables.scss" as *;

.footer-bottom-container{
    @include container;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 6.875rem;
    button{
        border: .0625rem solid $primary-color;
        padding: 1rem;
        background-color: transparent;
        color: white;
        font-weight: bold;
        &:hover{
            cursor: pointer;
            scale: 125%;
            border-radius: 10px;
        }
    }
    ul{
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        li{
            padding: .625rem;
            &:hover{
                cursor: pointer;
                border: 1px solid whitesmoke;
                border-radius: .625rem;
            }
        }
        .follow{
            color: $primary-color;
            font-size: x-large;
            font-weight: bold;
        }
    }
}

</style>