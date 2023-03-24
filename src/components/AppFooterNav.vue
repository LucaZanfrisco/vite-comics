<script>
export default {
    name: 'AppFooterNav',
    data(){
        return{
            listTopFooter: [
                {
                  image: 'src/assets/img/buy-comics-digital-comics.png',
                  name: 'DIGITAL COMICS'
                },
                {
                    image: 'src/assets/img//buy-comics-merchandise.png',
                    name: 'DC MERCHANDISE'
                },
                {
                    image: 'src/assets/img/buy-comics-subscriptions.png',
                    name: 'SUBSCRIPTION'
                },
                {
                    image:'src/assets/img/buy-comics-shop-locator.png',
                    name: 'COMIC SHOP LOCATOR'
                },
                {
                    image: 'src/assets/img/buy-dc-power-visa.svg',
                    name: 'DC POWER VISA'
                }
            ]
        }
    }
}
</script>

<template>
    <!-- Contenitore -->
    <div>
        <!-- Lista Nav Bar della parte superiore del footer -->
        <ul>
            <li v-for="list in listTopFooter">
                <img :src="list.image" :alt="list.name">
                <span>{{ list.name }}</span>
            </li>
        </ul>
        <!-- /Lista Nav Bar della parte superiore del footer -->
    </div>
</template>

<style lang="scss" scoped>
@use "../style/variables.scss" as *;

div{
    background-color: $primary-color;
    height: 9.6875rem;
    ul{
        @include container;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        li{
            display: flex;
            align-items: center;
            font-size: .8125rem;
            color: white;
            img{
                max-width: 3.4375rem;
                margin-right: .9375rem;
            }
        }
    }
}
</style>