<template>
    <div>
        <img :src="comicDetails.thumb" alt="">
        <h3>{{comicDetails.series}}</h3>
    </div>
</template>

<script>
    export default {
        name: 'ComicComp',
        props: {
            comicDetails: Object
        }
    }

</script>

<style scoped lang="scss">

    $size:calc((100% / 6) - 20px);

    div{
        width: $size;
        img{
            width: 100%;
        }
        padding-bottom: 20px;
    }

</style>