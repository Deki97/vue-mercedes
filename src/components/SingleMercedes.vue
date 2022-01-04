<template>
    <div class="single-mercedes">
        <div class="heading">
            <div class="title">
                <h3>{{ objectMercedes.model}}</h3>
            </div>
            
            <div class="description">
                <h4>{{ objectMercedes.description }}</h4>
            </div>
        </div>
        
        <div class="content">
            <div class="image">
                <img :src="objectMercedes.image" :alt="objectMercedes.model">
            </div>

            <div class="text">
                <div class="col-left">
                    <div class="price">
                        {{ objectMercedes.price }}
                    </div>

                    <div class="km">
                        <span>
                            Km:
                        </span>
                        {{ objectMercedes.km }}
                    </div>

                    <div class="fuel">
                        <span>
                            Alimentazione:
                        </span>
                        {{ objectMercedes.fuel }}
                    </div>
                </div>

                <div class="col-right">
                    <div class="hp">
                        <span>
                            Potenza:
                        </span>
                        {{ objectMercedes.hp }}
                    </div>

                    <div class="displacement">
                        <span>
                            Cilindrata:
                        </span>
                        {{ objectMercedes.displacement }}
                    </div>

                    <div class="color">
                        <span>
                            Colore:
                        </span>
                        {{ objectMercedes.color }}
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