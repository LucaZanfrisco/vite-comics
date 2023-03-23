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
        <!-- Componente Footer Superiore -->
        <AppFooterNav></AppFooterNav>
        <!-- Contenitore jumbotron con logo gigante e lista di info -->
        <div class="jumbotron">
            <div class="container-jumbo">
                <div class="container-info">
                    <div>
                        <ul>
                            <li><h3>DC COMICS</h3></li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movie</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <ul>
                            <li><h3>SHOP</h3></li>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li><h3>DC</h3></li>
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
                            <li><h3>SITES</h3></li>
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
        </div>
        <!-- /Contenitore jumbotron con logo gigante e lista di info -->
        <!-- Contenitore del footer inferiore -->
        <div class="bottom-container">
            <!-- Componente del footer inferiore -->
            <AppFooterBottom></AppFooterBottom>
        </div>
    </footer>   
    
    
</template>

<style lang="scss" scoped>
    @use '../style/variables.scss' as *;

    .jumbotron{
        background-image: url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 23.125rem;
        overflow-y: hidden;
        .container-jumbo{
            @include container;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
            height: 100%;
            .container-info{
                display: flex;
                ul{
                    margin-right: 1.6875rem;
                    margin-bottom: 1.75rem;
                    li{
                        font-size: 14px;
                        padding: .125rem;
                        color: $text-color;
                        &:hover{
                            cursor: pointer;
                            text-decoration: .125rem underline;
                        }
                        h3{
                            margin-bottom: 1.25rem;
                            font-size: medium;
                            color: white;
                        }
                    }
                }
            }
        }
    }
    .bottom-container{
        background-color: $secondary-color;
    }
</style>