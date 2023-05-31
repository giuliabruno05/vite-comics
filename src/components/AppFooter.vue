<script>

export default {
    name: "AppFooter"
}
</script>

<template>
    <footer>
        <section class="nav-footer">
            <div class="container">
                <div class="shortcut">
                    <ul>
                        <li class="title"><strong>DC COMICS</strong></li>
                        <li>Characters</li>
                        <li>Comics
                        </li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <li class="title"><strong>SHOP</strong></li>
                        <li>Games</li>
                        <li>Videos</li>
                    </ul>
                    <ul>
                        <li class="title"><strong>DC</strong></li>
                        <li>Tearms Of Use</li>
                        <li>Privacy Policy</li>
                        <li>Ad choice</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscripitions</li>
                        <li>Taalent Workshops</li>
                        <li>CPSC certtificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <li class="title"><strong>SITES</strong></li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
                <div class="logo-footer">
                    <img src="img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </section>
        <section class="row-footer">
            <div class="container">
                <button class="button"> SIGN-UP NOW!</button>
                <div class="icon">
                    <p class="follow"> <strong>FOLLOW US</strong></p>
                    <div class="image">
                        <img src="img/footer-facebook.png" alt="">
                    </div>
                    <div class="image">
                        <img src="img/footer-twitter.png" alt="">
                    </div>
                    <div class="image">
                        <img src="img/footer-youtube.png" alt="">
                    </div>
                    <div class="image">
                        <img src="img/footer-pinterest.png" alt="">
                    </div>
                    <div class="image">
                        <img src="img/footer-periscope.png" alt="">
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

.nav-footer {
    background-image: url("img/footer-bg.jpg");
    height: 260px;



    .container {
        display: flex;
        justify-content: space-between;

        .logo-footer {
            width: 350px;
            position: relative;
            top: -60px;
        }

        .shortcut {
            margin-top: 10px;
            display: flex;

            ul {
                margin: 0 10px;

                .title {
                    font-size: 1rem;
                    margin: 5px 0;
                }

                li {
                    color: #fff;
                    padding: 3px;
                    font-size: 0.6rem;
                    font-weight: 300;


                }
            }

        }


    }



}

.row-footer {
    height: 100px;
    background-color: $second-color;
    position: relative;
    z-index: 1000;


    .container {
        @include display-flex;

        .button {
            border-radius: 0%;
            border: 2px solid $theme-color;
            background-color: rgba(0, 0, 0, 0);
            color: #fff;
            font-size: 0.8rem;
            padding: 10px;
        }

        .icon {
            display: flex;


            .image {
                width: 20px;
                margin: 0 5px;
            }

            .follow {
                color: $theme-color;
                margin-right: 10px;
            }
        }
    }


}
</style>