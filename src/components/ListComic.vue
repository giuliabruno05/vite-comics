<script>
import CardComic from './CardComic.vue'
export default {
    name: "ListComic",
    components: {
        CardComic
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "ACTION COMICS",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "AMERICAN VAMPIRE 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "AQUAMAN",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "BATMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Batman_Beyond_v.1_1.webp",
                    "price": "$2.99",
                    "series": "BATMAN BEYOND",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Batman_Superman_Vol_1_1.webp",
                    "price": "$3.99",
                    "series": "BATMAN/SUPERMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Batman_Superman_Annual_Vol_2_1.webp",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Batman_The_Joker_War_Zone_Vol_1_1.webp",
                    "price": "$5.99",
                    "series": "BATMAN: THE JOKER WAR ZONE",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Batman_Three_Jokers_Collected.webp",
                    "series": "BATMAN: THREE JOKERS",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.webp",
                    "price": "$4.99",
                    "series": "BATMAN: WHITE KNIGHT PRESENTS: HARLEY QUIIN",
                    "type": "comic book"
                },
                {
                    "thumb": "/img/Catwoman_Vol_2_1.webp",
                    "price": "$16.99",
                    "series": "CATWOMAN",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <div class="box-comic">
        <CardComic v-for="(comic, index) in comics" :key="index" :details="comic" />
    </div>
</template>


<style lang="scss" scoped>
.box-comic {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding-top: 40px;
    gap: 5px;

}
</style>