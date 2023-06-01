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
                    <div>
                        <ul>
                            <li class="title"><strong>DC COMICS</strong></li>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a>
                            </li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">Tv</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li>News</li>
                        </ul>
                        <ul>
                            <li class="title"><strong>SHOP</strong></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                        </ul>
                    </div>
                    <ul>
                        <li class="title"><strong>DC</strong></li>
                        <li><a href="#">Tearms Of Use</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Ad choice</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscripitions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC certtificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                    <ul>
                        <li class="title"><strong>SITES</strong></li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
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
                        <a href="#"><img src="img/footer-facebook.png" alt="logo facebook"></a>
                    </div>
                    <div class="image">
                        <a href="#"><img src="img/footer-twitter.png" alt="logo twitter"></a>
                    </div>
                    <div class="image">
                        <a href="#"><img src="img/footer-youtube.png" alt="logo youtube"></a>
                    </div>
                    <div class="image">
                        <a href="#"><img src="img/footer-pinterest.png" alt="logo pinterest"></a>
                    </div>
                    <div class="image">
                        <a href="#"><img src="img/footer-periscope.png" alt="logo periscope"></a>
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
                    color: #fff;
                }

                li {
                    padding: 3px;
                    font-size: 0.6rem;
                    font-weight: 300;

                    a {
                        color: #fff;
                    }

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