<script>

export default {
    name: 'AppMain',
}

</script>


<template>

    <main>
        <div class="jumbotron"></div>
        <div class="content">
            <div class="my-container">
                <h3>-- Content goes here --</h3>
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

    h3{
        color: white;
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