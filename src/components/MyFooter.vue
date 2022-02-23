<template>
   <footer>
     <div class="footer-container">
         <div class="container">

            <!-- Row -->
            <div class="row">
                <div class="link">
                    <div class="col">
                        <h3>DC Comics</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                            </ul>
                        </div>
                        <!-- Negozio -->
                        <h3>Shop</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                            </ul>
                        </div>
                    </div>
                    <!-- Parte DC -->
                    <div class="col">
                        <h3>DC</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">Terms of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li><a href="#">Talent Workshops</a></li>
                            <li><a href="#">CPSC Certificates</a></li>
                            <li><a href="#">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="#">Contact Us</a></li>
                            </ul>
                        </div>
                    </div>
                    <!-- Link dei siti -->
                    <div class="col">
                        <h3>Sites</h3>
                        <div class="list">
                            <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <div class="container-logo-right">
                <img class="logo-right" src="../assets/img/dc-logo-bg.png" alt="">
            </div>
             

         </div>
     </div>

    <!-- Icone nel footer -->
    <div class="footer-icon">
      <div class="container">
        <div class="row">

          <button>SIGN-UP NOW!</button>

          <div class="social">
            <a href="#">FOLLOW US</a>
            <img src="../assets/img/footer-facebook.png" alt="Facebook">
            <img src="../assets/img/footer-twitter.png" alt="Twitter">
            <img src="../assets/img/footer-youtube.png" alt="YouTube">
            <img src="../assets/img/footer-pinterest.png" alt="Pinterest">
            <img src="../assets/img/footer-periscope.png" alt="Periscope">
          </div>
        </div>
       </div>
    </div>

   </footer>
</template>

<script>
export default {
  name: 'MyFooter'
}
</script>

<style scoped lang="scss">
    @import "../assets/style/variabili.scss";
    footer {
        .footer-container {
            padding: 30px 0px;
            background-image: url('../assets/img/footer-bg.jpg');
            background-repeat: no-repeat;
            background-size: cover;
            overflow: hidden;
            height: 400px;
            
            .container {
                position: relative;
            }
            .link {
                display: flex;
                .col {
                    width: 170px;
                    h3 {
                        color: $light;
                        text-transform: uppercase;
                        margin: 20px 0px;
                    }
                    .list {
                        ul {
                            list-style: none;
                            li {
                                margin: 5px 0px;
                                a {
                                    font-size: 12px;
                                    text-decoration: none;
                                    color: #959595;
                                    &:hover {
                                        color: $light;
                                    }
                                }
                            }
                        }
                    }
                }
            }
            .container-logo-right {
                position: absolute;
                top: -25%;
                right: 0;
                .logo-right {
                height: 500px;
                }   
            }
        }
        .footer-icon {
            background-color: $footerBg;
            .row {
                justify-content: space-between;
                button {
                    border: 2px solid $primaryColor;
                    background-color: $footerBg;
                    color: $light;
                    padding: 12px;
                    margin: 20px 0px;
                    font-size: 16px;
                    cursor: pointer;
                    &:hover {
                        border: 2px solid $primaryColorHover;
                    }
                }
                .social {
                    display: flex;
                    align-items: center;
                    img {
                        margin: 0px 10px;
                        &:hover {
                            // uso un webkit filter?
                            -webkit-filter: contrast(175%) brightness(3%);
                        }
                    }
                    a {
                        text-decoration: none;
                        color: $primaryColor;
                        font-weight: bold;
                        margin-right: 5px;
                        &:hover {
                        color: $primaryColorHover;
                    }
                    }
                }
            }
        }
    }
  
</style>