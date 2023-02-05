<script>

export default {
    name: 'AppFooter',
}

</script>


<template>

    <footer>
        <div class="footer-up">
            <div class="row my-container">
                <div class="col-6">
                    <div class="row">
                        <div class="col-3">
                            <ul>
                                <li>
                                    <h6>DC COMICS</h6>
                                </li>
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li> 
                            </ul>
                            <ul>
                                <li>
                                    <h6>SHOP</h6>
                                </li>
                                <li>Shop DC</li>
                                <li>Shop DC Collectibles</li>
                            </ul>
                        </div>
                        <div class="col-3">
                            <ul>
                                <li>
                                    <h6>DC</h6>
                                </li>
                                <li>Terms Of Use</li>
                                <li>Privacy policy (New)</li>
                                <li>Ad Choices</li>
                                <li>Advertising</li>
                                <li>Jobs</li>
                                <li>Subscriptions</li>
                                <li>Talent Workshops</li>
                                <li>CPSC Certificates</li>
                                <li>Ratings</li>
                                <li>Shop Help</li> 
                            </ul>
                        </div>
                        <div class="col-3">
                            <ul>
                                <li>
                                    <h6>SITES</h6>
                                </li>
                                <li>DC</li>
                                <li>MAD Magazine</li>
                                <li>DC Kids</li>
                                <li>DC Univers</li>
                                <li>DC Power Visa</li> 
                            </ul>
                        </div>
                        <div class="col-3">

                        </div>
                    </div>
                </div>
                <div class="col-6 special"></div>
            </div>
        </div>

        <div class="footer-bottom">
            <div class="my-container">
                <div class="sign-up">
                    <button>SIGN-UP NOW!</button>
                </div>

                <div class="socials">
                    <span class="blue">FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="Facebook">
                    <img src="../assets/img/footer-twitter.png" alt="Twitter">
                    <img src="../assets/img/footer-youtube.png" alt="YouTube">
                    <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="Periscope">
                </div>
            </div>
        </div>

    </footer>
</template>


<style lang="scss" scoped>

footer{
    width: 100%;
    height: auto;
}
.footer-up{
    background-image: url("../assets/img/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    color: white;
    height: auto;

    div.row{

        ul{
            list-style: none;
            padding: 10px 0;
            
            h6{
                font-weight: 1000;
                color: white;
            }

            li{
                color: rgba(193, 193, 193, 0.561);
            }


        }

        div.col-6.special{
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-position: center;
        }
    }
}

.footer-bottom{
    padding: 20px 0;

    div{
        display: flex;
        justify-content: space-between;
        align-items: center;

        button{
        padding: 7px;
        color: white;
        }

        span{
            padding: 0 10px;
        }

        img{
            padding: 0 7px;
        }
    }
    


    
}
</style>