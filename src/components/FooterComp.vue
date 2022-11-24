<template>
    <div id="mainDiv">
        <!-- main footer -->
        <section id="mainFooter">
            <div class="container-70 flex-bw f-wrap">
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
                    
                        <h2>SHOP</h2>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                        
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
                <div id="bg-logo">
                    
                </div>
            </div>
        </section>
        <!-- bottom footer -->
        <div id="bottom">
            <div class="container-70">
                <section>
                    <button>SIGN-UP NOW</button>
                </section>
                <section>
                    <a href="#">FOLLOW US</a>
                    <img src="../assets/footer-facebook.png" alt="">
                    <img src="../assets/footer-twitter.png" alt="">
                    <img src="../assets/footer-youtube.png" alt="">
                    <img src="../assets/footer-pinterest.png" alt="">
                    <img src="../assets/footer-periscope.png" alt="">

                </section>                
            </div>
        </div>
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

    #mainDiv{
        height: calc(100% - ($hm + ($hs * 2)));
    }

    #mainFooter{
        height:calc(100% - $hs );
        background-image: url("../assets/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
    }

    #bottom{
        background-color: rgb(24, 22, 22);
        height: $hs;
        div{
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
            section{

                *{
                    vertical-align: middle;
                }

                button{
                    padding: 15px;
                    background: none;
                    border: 2px solid blue;
                    font-weight: bolder;
                }

                a{
                    text-decoration: none;
                    color: blue;
                    cursor: pointer;
                    font-weight: bolder;
                    font-size: 20px;
                }

                img{
                    margin: 0 13px;
                    cursor: pointer;
                }
            }
        }
    }

    h2{
        margin: 25px 0;
    }
    
    #lists{
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        ul{
            margin: 0 20px;
        }
    }

    li{
        margin: 8px 0;
        opacity: 0.5;
    }

    li:hover{
        opacity: 1;
        cursor: pointer;
    }

    #bg-logo{
        position: relative;
        background-image: url("../assets/dc-logo-bg.png");
        width: 50%;
        aspect-ratio: 1;
        background-repeat: no-repeat ;
    }
</style>
