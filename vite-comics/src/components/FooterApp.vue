<script>

export default {
  name: "FooterApp"
}
</script>

<template>
    <div class="container">

        <div>
            <ul>
                <li>
                    <i href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="Logo Dc Comics">
                        <p>digital comics</p>
                    </i>
                </li>
                <li>
                    <i href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="Logo Dc Merchandise">
                        <p>dc merchandise</p>
                    </i>
                </li>
                <li>
                    <i href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="Logo Dc Subscriptions">
                        <p>subscription</p>
                    </i>
                </li>
                <li>
                    <i href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="Logo Dc Locator">
                        <p>comic shop locator</p>
                    </i>
                </li>
                <li>
                    <i href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="Logo Dc Power Visa">
                        <p>dc power visa</p>
                    </i>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;
.container{
    background-color: #0282f9;
    width: 100%;
    padding: 30px;

    div{
        width: 80%;
        margin: 0 auto;

        ul{
            list-style-type: none;
            display: flex;
            justify-content: space-between;

            li{
                color: #ffffff;
                text-transform: uppercase;

                i{
                    display: flex;
                    width: 50px;
                    gap: 10px;
                    align-items: center;

                    &:hover{
                        cursor: pointer;
                        
                    }

                    img{
                        width: 100%;
                    }
                }
            }
        }
    }
}
</style>