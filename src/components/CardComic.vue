
<script>
export default {
    name: "CardComic",
    props: {
        details: Object
    }
}
</script>
<template>
    <div class="card-comic">

        <div class="image"><img :src="details.thumb" :alt="details.type">
        </div>
        <div class="text">
            <h4>{{ details.series }}</h4>
        </div>

    </div>
</template>
<style lang="scss" scoped>
.card-comic {
    font-size: 0.8rem;
    width: 15%;
    margin-bottom: 30px;


    h4 {
        color: #fff;
        font-size: 0.7rem;
        margin-top: 5px;
    }

    .image img {
        height: 145px;
        object-position: top;
        object-fit: cover;
    }



}
</style>