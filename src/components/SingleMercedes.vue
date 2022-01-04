<template>
    <div class="single-mercedes">
        <div class="heading">
            <div class="title">
                <h3>Mercedes Classe A</h3>
            </div>
            
            <div class="description">
                <h4>250 e eq-power premium auto</h4>
            </div>
        </div>
        
        <div class="content">
            <div class="image">
                <img src="https://trivellato.media.weicola.it/trivellato/wrap360/medium/-/+2021+11+22+V031600_619ba39d4aa56.jpg/49993b7f3669501199ac836f6821dcea.jpg" alt="Mercedes Classe A">
            </div>

            <div class="text">
                <div class="col-left">
                    <div class="price">
                        € 45.900
                    </div>

                    <div class="km">
                        <span>
                            Km:
                        </span>
                        0
                    </div>

                    <div class="fuel">
                        <span>
                            Alimentazione:
                        </span>
                        Elettrica
                    </div>
                </div>

                <div class="col-right">
                    <div class="hp">
                        <span>
                            Potenza:
                        </span>
                        218 CV
                    </div>

                    <div class="displacement">
                        <span>
                            Cilindrata:
                        </span>
                        1.332
                    </div>

                    <div class="color">
                        <span>
                            Colore:
                        </span>
                        Nero
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'SingleMercedes',
    props: {
        objectMercedes: Object
    }
}
</script>


<style lang="scss" scoped>
@import '../style/variables.scss';

.single-mercedes {
    border: 1px solid lighten($page-secondary-color, 10%);
    border-radius: 10px;
    padding: 10px 20px;
    margin: 10px 0;
    transition: 0.2s;
    
    &:hover {
        box-shadow: 2px 2px 10px lighten($page-secondary-color, 10%);
        transition: 0.2s ease-in-out;
        cursor: pointer;
        transform: rotate(0.2deg);
    }

    .heading {
        margin: 10px 0;

        .title {
            h3 {
                font-size: 22px;
            }
        }

        .description {
            h4 {
                color: lighten($page-primary-color, 40%);
                margin-top: 5px;
            }
        }
    }
    .content {
        display: flex;
        

        .image {
            img {
                width: 280px;
            }
        }

        .text {
            display: flex;

            span {
                font-weight: bold;
            }

            .col-left {
                display: flex;
                flex-direction: column;
                justify-content: space-around;
                margin: 0 20px;

                .price {
                    font-weight: bold;
                }
            }

            .col-right {
                display: flex;
                flex-direction: column;
                justify-content: space-around;
                margin: 0 20px;
            }

            .col-left div,
            .col-right div {
                border-bottom: 1px solid lighten($page-primary-color, 40%);
                padding: 5px 0;
            }
        }
    }
}
</style>