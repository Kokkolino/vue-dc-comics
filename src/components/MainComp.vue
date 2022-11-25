<template>
    <div>
        <!-- jumbodrillo -->
        <section id="jumbotron">
        </section>
        <!-- comics section -->
        <section id="comicsSec" class="black">
            <div id="bookshelf" class="container-70 h-100">
                <ComicComp
                v-for="(elem, index) in comics" 
                :key="index" 
                :comicDetails="elem"/>
            </div>
            <button></button>
        </section>
        <!-- blue section -->
        <section id="bluesec" class="blue">
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

import ComicComp from './ComicComp.vue'


    export default {
        name: 'MainComp',
        components:{
            ComicComp
        },
        data(){
         return{
            comics:[
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                  "price": "$19.99",
                  "series": "Action Comics",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                  "price": "$3.99",
                  "series": "American Vampire 1976",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                  "price": "$16.99",
                  "series": "Aquaman",
                  "type": "graphic novel"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                  "price": "$2.99",
                  "series": "Batgirl",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                  "price": "$3.99",
                  "series": "Batman",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                  "price": "$2.99",
                  "series": "Batman Beyond",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                  "price": "$3.99",
                  "series": "Batman/Superman",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                  "price": "$4.99",
                  "series": "Batman/Superman Annual",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                  "price": "$5.99",
                  "series": "Batman: The Joker War Zone",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                  "price": "$6.99",
                  "series": "Batman: Three Jokers",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                  "price": "$4.99",
                  "series": "Batman: White Knight Presents: Harley Quinn",
                  "type": "comic book"
               },
               {
                  "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                  "price": "$16.99",
                  "series": "Catwoman",
                  "type": "graphic novel"
               }
            ]
         }
      }

}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/var.scss";

    div{
        z-index: 1;
    }

    #jumbotron{
        background-image: url("../assets/jumbotron.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        height: 400px;
    }

    #comicsSec{
        height: 900px;
    }

    #bookshelf{
        padding: 20px 0;;
        height: 500px;
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
    }

    #bluesec{
        height: $hm;
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
