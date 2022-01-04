<template>
    <main>
        <Banner />

        <div class="container">
            <h2>Le nostre vetture</h2>
            <SingleMercedes v-for="(item, index) in cars" :key="index" :objectMercedes="item"/>
        </div>

    </main>
</template>


<script>
import Banner from './Banner.vue';
import SingleMercedes from './SingleMercedes.vue';

export default {
    name: 'Main',
    components: {
        Banner,
        SingleMercedes
    },
    data: function() {
        return {
            cars: [
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+11+22+V031600_619ba39d4aa56.jpg/49993b7f3669501199ac836f6821dcea.jpg",
                   "model": "Mercedes Classe A",
                   "description": "250 e eq-power premium auto",
                   "price": "€ 45.900",
                   "km": "0",
                   "fuel": "Elettrica",
                   "hp": "218 CV",
                   "displacement": "1.332",
                   "color": "Nero"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+09+27+V034181_6151c1a18eb64.jpg/5f7390ed977131bdfbab0869bad310fa.jpg",
                   "model": "Mercedes Classe B",
                   "description": "250 e plug-in hybrid(e-eq-power) premium auto",
                   "price": "€ 43.900",
                   "km": "0",
                   "fuel": "Elettrica",
                   "hp": "218 CV",
                   "displacement": "1.332",
                   "color": "Blu"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+12+10+V035748_61b334aaeafa3.jpg/18addba7647582a6c9511672fe318929.jpg",
                   "model": "Mercedes Classe C Berlina",
                   "description": "220 d premium auto",
                   "price": "€ 38.000",
                   "km": "34.300",
                   "fuel": "Diesel",
                   "hp": "194 CV",
                   "displacement": "1.950",
                   "color": "Argento"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+11+30+V034571_61a6056a6edeb.jpg/6f52446ecd86659da75e892342ffa85f.jpg",
                   "model": "Mercedes Classe E Berlina",
                   "description": "E 220d Auto AMG Line",
                   "price": "€ 35.800",
                   "km": "76.535",
                   "fuel": "Diesel",
                   "hp": "194 CV",
                   "displacement": "1.950",
                   "color": "Argento"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+10+28+V034225_617a59efd0b8b.jpg/d566707db988096a0fb74310ade58225.jpg",
                   "model": "Mercedes CLA Shooting Brake",
                   "description": "200 d premium 4matic auto fl",
                   "price": "€ 28.000",
                   "km": "96.650",
                   "fuel": "Diesel",
                   "hp": "136 CV",
                   "displacement": "2.143",
                   "color": "Nero"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+10+27+V034719_617994da831e4.jpg/4cccdbf9b90375588240cf3658e90505.jpg",
                   "model": "Mercedes CLS",
                   "description": "coupe 400 d premium plus 4matic auto",
                   "price": "€ 125.627",
                   "km": "0",
                   "fuel": "Diesel",
                   "hp": "330 CV",
                   "displacement": "2.925",
                   "color": "Grigio"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+12+23+V033216_61c45e198e817.jpg/f5d8d46ee23d94cad49555661bfb3f1b.jpg",
                   "model": "Mercedes GLA",
                   "description": "200 d premium auto",
                   "price": "€ 49.888",
                   "km": "0",
                   "fuel": "Diesel",
                   "hp": "150 CV",
                   "displacement": "1.950",
                   "color": "Bianco"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+12+21+V036632_61c1fb3d5a256.jpg/fc6451de05f3c5a5fd051d78e40cd877.jpg",
                   "model": "Mercedes GLE Coupè",
                   "description": "gle coupe 350 de plug-in hybrid(e eq-power) premium pro 4matic auto",
                   "price": "€ 106.417",
                   "km": "0",
                   "fuel": "Ibrido",
                   "hp": "194 CV",
                   "displacement": "1.950",
                   "color": "Bianco"
                },
                {
                   "image": "https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+11+29+V035644_61a5246a0fafe.jpg/70011e3317e8c4b55e9d1c7a3bf37ccf.jpg",
                   "model": "AMG GT",
                   "description": "4.0 462cv auto",
                   "price": "€ 79.800",
                   "km": "47.050",
                   "fuel": "Benzina",
                   "hp": "462 CV",
                   "displacement": "3.982",
                   "color": "Argento"
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

main {
    .container {
        padding: 50px 0;

        h2 {
            font-size: 36px;
            margin: 50px 0;
            color: lighten($page-secondary-color, 10%);
        }
    }
}
</style>