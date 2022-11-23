<template>
    <div>
        <!-- black badge -->
        <section class="height-row bg-black flex-align">
            <div class="container-70">
                <h1>-->Content here pls</h1>
            </div>
        </section>
        <!-- blue section -->
        <section class="bg-blue">
            <div class="container-70 flex-bw h-100">
                <ul class="horizontal-ul">
                    <li>
                        <img src="../assets/buy-comics-digital-comics.png" alt="">
                        <span>
                            DIGITAL COMICS
                        </span> 
                    </li>
                    <li>
                        <img src="../assets/buy-comics-merchandise.png" alt="">
                        <span>
                            DC MERCHANDISE
                        </span> 
                    </li>
                    <li>
                        <img src="../assets/buy-comics-subscriptions.png" alt="">
                        <span>
                            SUBSCRIPTION
                        </span> 
                    </li>
                    <li>
                        <img src="../assets/buy-comics-shop-locator.png" alt="">
                        <span>
                            COMIC SHOP LOCATOR
                        </span> 
                    </li>
                    <li>
                        <img src="../assets/buy-dc-power-visa.svg" alt="">
                        <span>
                            DC POWER VISA
                        </span> 
                    </li>
                </ul>
            </div>
        </section>
    </div>
</template>
  
<script>
    export default {
        name: 'MainComp',
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/var.scss";

    div{
        z-index: 1;
    }
    .bg-black{
        background-color: black;
    }


    .bg-blue{
        height: $hm;
        background-color: rgb(44, 160, 255);
    }

    li{
        margin: 0 20px;
        display: flex;
        align-items: center;
        img{
            width: 45px;
            max-height: 60px;
            margin: 0 10px;
        }
    }

    li:hover{
        cursor: pointer;
    }
</style>
