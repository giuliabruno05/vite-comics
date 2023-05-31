<script>

export default {
    name: "AppMain"
}
</script>

<template>
    <main>
        <section class="coming-soon">
            <div class="container">
                <h2>Content goes here</h2>
            </div>
        </section>
        <section class="shop">
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
    background-color: $black;
    height: 100px;
    color: #fff;
    padding: 20px;
}

.shop {
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