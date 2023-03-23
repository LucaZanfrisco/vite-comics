<script>
export default {
    name: 'AppFooterNav',
}
</script>

<template>
    <!-- Contenitore -->
    <div>
        <!-- Lista Nav Bar della parte superiore del footer -->
        <ul>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
                <span>DIGITAL COMICS</span>
            </li>
            <li>
                <img src="../assets/img//buy-comics-merchandise.png" alt="dc-merch"> 
                <span>DC MERCHANDISE</span>
            </li>
            <li>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="subs">
                <span>SUBSCRIPTION</span>
            </li>
            <li>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator">
                <span>COMIC SHOP LOCATOR</span>
            </li>
            <li>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="power-visa">
                <span>DC POWER VISA</span>
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
                max-height: 3.4375rem;
                margin-right: .9375rem;
            }
        }
    }
}
</style>