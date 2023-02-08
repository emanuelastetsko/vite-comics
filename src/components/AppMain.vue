<script>

export default {
    name: 'AppMain',
    data(){
        return{
            comics: [
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
        };
    }
}

</script>


<template>

    <main>
        <div class="jumbotron"></div>
        <div class="content">
            <div class="my-container">
                <div class="label">
                    <span class="label-span">CURRENT SERIES</span>
                </div>
                <div class="cards">
                    <div class="card" v-for="comic in comics">
                        <div class="comic-img">
                            <img :src="comic.thumb" :alt="comic.series" class="img">
                        </div>
                        <div class="comic-title">
                            <h6>{{ comic.series.toUpperCase() }}</h6>
                        </div>
                    </div>
                </div>
                <div class="button">
                    <button>LOAD MORE</button>
                </div>
            </div>
        </div>
        <div class="section">
            <div class="my-container">
                <div class="my-section">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                    <span>DIGITAL COMICS</span>
                </div>
                <div class="my-section">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="Merchandise">
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="my-section">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="Subscriptions">
                    <span>SUBSCRIPTION</span>
                </div>
                <div class="my-section">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="Shop Locator">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
                <div class="my-section unique">
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="Power Visa" class="special">
                    <span>DC POWER VISA</span>
                </div>
            </div>
        </div>
    </main>

</template>


<style lang="scss" scoped>

.jumbotron{
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    height: 350px;
}
.content{
    background-color: black;
    padding: 50px 0;

    
}

.cards{
    display: flex;
    flex-wrap: wrap;

    .card{
        background-color: black;
        width: calc(100% / 6);
        padding: 10px;
        color: white;

        .comic-title{
            margin-top: 10px;
        }
    }
}

.section{
    padding: 30px 0;
    color: white;

    div.my-container{
        display: flex;
        align-items: center;
        justify-content: space-around;

            div.my-section{
                
                img{
                    width: 40px;
                    height: 50px;
                    margin-right: 10px;
                }

                span{
                    font-size: 0.9em;
                }
            }
        
    }
}

</style>