<script>
import ListComic from './ListComic.vue'
export default {
    name: "AppMain",
    components: {
        ListComic
    },
}
</script>

<template>
    <main>
        <section class="coming-soon">
        </section>
        <section>
            <div class="list-card">
                <div class="container">
                    <ListComic />
                    <div class="label">
                        CURRENT SERIES
                    </div>
                    <div class="labelTwo">
                        LOAD MORE
                    </div>
                </div>

            </div>
        </section>
        <section class="other-Link">
            <div class="container">
                <div class="card">
                    <div class="image">
                        <img src="img/buy-comics-digital-comics.png" alt="">
                    </div>
                    <div class="text-image">
                        <p>DIGITAL COMICS</p>
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div class="text-image">
                        <p>DC MERCHANDISE</p>
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="text-image">
                        <p>SUBSCRIPTION</p>
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="text-image">
                        <p>COMIC SHOP LOCATORE</p>
                    </div>
                </div>
                <div class="card">
                    <div class="image">
                        <img src="img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="text-image">
                        <p>DC POWER VISA</p>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

.coming-soon {
    background-image: url("img/jumbotron.jpg");
    background-size: cover;
    height: 250px;
    position: relative;

}



.list-card {
    background-color: #1c1c1c;

    .container {
        padding-bottom: 10px;
    }

    .label {
        @include label;
        position: absolute;
        top: 335px;
        background-color: $theme-color;
    }

    .labelTwo {
        @include label;
        background-color: $theme-color;
        margin: 0 auto;

    }

}


.other-Link {
    background-color: $theme-color;
    height: 100px;
    position: relative;
    z-index: 1000;


    .container {
        @include display-flex;


        .card {
            display: flex;
            align-items: center;

            font-size: 0.8rem;
            height: 100%;

            .image {
                width: 30px;

            }

            .text-image {
                margin: 0 10px;
                color: #fff;
            }
        }

    }


}
</style>