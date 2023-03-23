<script>
import AppFooterNav from './AppFooterNav.vue';
import AppFooterBottom from './AppFooterBottom.vue';
    export default{
        name: 'AppFooter',
        components: {
            AppFooterNav,
            AppFooterBottom,
        }
    }
</script>

<template>
    <footer>
        <AppFooterNav></AppFooterNav>
    </footer>   
    <div>
        <div>
            <div>
                <ul>
                    <li>DC COMICS</li>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movie</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>
                <ul>
                    <li>SHOP</li>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
            </div>
            <div>
                <ul>
                    <li>DC</li>
                    <li>Terms of Use</li>
                    <li>Privacy policy(New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Show Help</li>
                    <li>Contac Us</li>
                </ul>
            </div>
            <div>
                <ul>
                    <li>SITES</li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        </div>
        <div>
            <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-big">
        </div>
    </div>
    <div>
        <AppFooterBottom></AppFooterBottom>
    </div>
</template>

<style lang="scss" scoped>
    @use '../style/variables.scss' as *;


</style>