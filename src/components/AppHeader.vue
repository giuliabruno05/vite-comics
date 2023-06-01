<script>

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#"
                },
                {
                    text: "COMICS",
                    url: "#"
                },
                {
                    text: "MOVIES",
                    url: "#"
                },
                {
                    text: "TV",
                    url: "#"
                },
                {
                    text: "GAMES",
                    url: "#"
                },
                {
                    text: "COLLECTIBLES",
                    url: "#"
                },
                {
                    text: "VIDEOS",
                    url: "#"
                },
                {
                    text: "FANS",
                    url: "#"
                },
                {
                    text: "NEWS",
                    url: "#"
                },
                {
                    text: "SHOP",
                    url: "#"
                }
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="img/dc-logo.png" alt="">
            </div>
            <nav class="navigazione">
                <ul>
                    <li v-for="link in links">
                        <a :href="link.url" :class="link.current ? 'active' : ''">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

header {
    height: 100px;

    .container {
        @include display-flex;

        .logo {
            width: 70px;
        }

        ul {
            display: flex;

            li {
                padding: 10px;

                a {
                    color: $second-color;
                    font-size: 0.8rem;

                    &.active,
                    &:hover {
                        color: $theme-color;
                    }
                }
            }
        }
    }


}
</style>