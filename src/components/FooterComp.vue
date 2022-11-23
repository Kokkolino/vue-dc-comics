<template>
    <div>
        <!-- main footer -->
        <section id="mainFooter">
            <div class="container-70">
                <section id="lists" class="f-wrap">
                    <ul>
                        <h2>DC COMICS</h2>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <ul>
                            <h2>SHOP</h2>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </ul>
                    <ul>
                        <h2>DC</h2>
                        <li>Terms Of Use</li>
                        <li>Privacy</li>
                        <li>Ad Choice</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                    <ul>
                        <h2>SITES</h2>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>

                </section>
                <section>

                </section>
            </div>
        </section>
        <!-- bottom footer -->
        <section id="bottom" class="height-row">

        </section>
    </div>
</template>

<script>
    export default {
        name: 'FooterComp',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/var.scss"; 

    div{
        height: calc(100% - ($hm + ($hs * 3)));
    }

    #mainFooter{
        height: 100%;
        background-image: url("../assets/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
    }

    #bottom{
        background-color: rgb(24, 22, 22);
    }

    h2{
        margin: 25px 0;
    }
    
    #lists{
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
    }

    li{
        margin: 8px 0;
        opacity: 0.5;
    }

    li:hover{
        opacity: 1;
        cursor: pointer;
    }

</style>
