<script>

export default {
  name: "Footer"
}
</script>

<template>
<div class="container-second">
    <div>
        <div class="list">

            <ul>
                <h4>DC COMICS</h4>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
                <br>
                <h4>SHOP</h4>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
            </ul>
            
            <ul>
                <h4>DC</h4>
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
                <li>Contact Us</li>
            </ul>

            <ul>
                <h4>SITES</h4>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
            </ul>
        </div>
        <figure>

        </figure>
    </div>
</div>

<div class="container-third">
    <div class="container-fourth">
        <button>SIGN-UP NOW</button>
        <div>
            <span>FOLLOW US</span>
            <i>
                <img src="../assets/img/footer-facebook.png" alt="Facebook icon">
            </i>
            <i>
                <img src="../assets/img/footer-twitter.png" alt="Twitter icon">
            </i>
            <i>
                <img src="../assets/img/footer-youtube.png" alt="Youtube icon">
            </i>
            <i>
                <img src="../assets/img/footer-pinterest.png" alt="Pinterest icon">
            </i>
            <i>
                <img src="../assets/img/footer-periscope.png" alt="Periscope icon">
            </i>
        </div>
    </div>
</div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;


.container-second{
    width: 100%;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    div{
        display: flex;
        justify-content: space-between;
        width: 80%;
        margin: 0 auto;
        .list{
            display: flex;
            justify-content: flex-start;
            gap: 40px;
            margin: 40px 0;

            ul{ 
                list-style-type: none;
    
                h4{
                    padding-bottom: 15px;
                    font-size: 25px;
                    color: #ffffff;
                    user-select: none;
                }

                li{
                    cursor: pointer;
                    line-height: 2em;
                    color: #808080;
                
                    &:hover{
                        color: #ffffff;
                    }
                }
            }
        }

        figure{
            width: 100%;
            background-repeat: no-repeat;
            background-position: center;
            background-image: url("../assets/img/dc-logo-bg.png");
        }
    }
    
}

.container-third{

    width: 100%;
    background-color: #333333;
    padding: 30px 0;
    .container-fourth{

        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        button{
            padding: 10px 15px;
            color: #ffffff;
            background-color: #303030;
            border: 5px solid #0282f9;
            cursor: pointer;
            -webkit-box-shadow: 5px 5px 10px 5px #000000; 
            box-shadow: 5px 5px 10px 5px #000000;

            &:hover{
                transform: scale(1.1);
            }
        }

        div{
            display: flex;
            gap: 20px;
            align-items: center;

            span{
                color: #0282f9;
                font-weight: bold;
                &:hover{
                    cursor: pointer;
                    transform: scale(1.1);
                }
            }

            i{
                width: 20px;

                img{
                    width: 100%;
                    &:hover{
                        transform: scale(1.3);
                        cursor: pointer;
                    }
                }
            }
        }
    }
}
</style>