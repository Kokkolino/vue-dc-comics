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

    $size:calc((100% / 6) - 5px);

    div{
        width: $size;
        height: calc(  $size + 30px );
    }

</style>