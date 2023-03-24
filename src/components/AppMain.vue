<script>
import CardsElement from './CardsElement.vue';
export default {
    name: 'AppMain',
    components: {
        CardsElement,
    },
    data() {
        return {
            comicsList: [
                {
                    "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$19.99",
                    "series": "DC'S LEGION OF BLOOM",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "THE FLASH",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
                    "price": "$16.99",
                    "series": "NIGHTWING",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
                    "price": "$2.99",
                    "series": "BATMAN/SUPERMAN: WORLD'S FINEST",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/CTW_Cv53_05311_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "CATWOMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
                    "price": "$2.99",
                    "series": "BLACK ADAM",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "SUPERMAN: LOST",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SUPES_Cv2_00211_DIGITAL.jpg?w=640",
                    "price": "$4.99",
                    "series": "SUPERMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
                    "price": "$5.99",
                    "series": "ROBIN VOL. 3: SECRETS AND SHADOWS ",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/HQv3%20%28%20Cover%29.jpg?w=640",
                    "price": "$6.99",
                    "series": "HARLEY QUINN VOL. 3: VERDICT",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/MULTVTJ%20%28COVER%29.jpg?w=640",
                    "price": "$4.99",
                    "series": "MULTIVERSITY: TEEN JUSTICE",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/WW_Cv797_79711_DIGITAL.jpg?w=640",
                    "price": "$16.99",
                    "series": "WONDER WOMAN",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <main>
        <img src="../assets/img/jumbotron.jpg" alt="jumbotron" class="jumbotron">
        <div class="products-container">
            <h3>CURRENT SERIES</h3>
            <div class="products">
                <CardsElement class="product" v-for="comic in comicsList" :image="comic.thumb" :name="comic.series"></CardsElement>
            </div>
            <div class="more">
                <button class="more-load" type="button">LOAD MORE</button>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/variables.scss' as *;

main {
    background-color: black;
    padding-bottom: 1.25rem;
    .jumbotron{
        height: 400px;
        object-fit: cover;
        object-position: top;
    }
    .products-container {
        @include container;
        height: 100%;
        color: white;
        h3{
            background-color: $primary-color;
            display: inline-block;
            padding: 1.0625rem 1.875rem;
            font-size: 1.4rem;
            position: relative;
            bottom: 1.6875rem
        }
        .products {
            display: flex;
            flex-wrap: wrap;
            margin: 1.0625rem -0.625rem 3.4375rem;

            .product {
                flex-basis: calc(100% / 6 - 1.25rem);
                margin: 10px;
                :deep(.title) {
                    margin-top: 1.375rem;
                }
            }
        }
        .more{
            text-align: center;
        }
        .more-load {
            text-align: center;
            background-color: $primary-color;
            border: none;
            padding: 12px 55px;
            font-weight: bold;
            color: inherit;
            &:hover{
                cursor: pointer;
                scale: 1.1;
            }
        }
    }
}
</style>