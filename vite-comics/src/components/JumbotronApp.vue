<script>

export default {
  name: "JumbotronApp"
}
</script>

<template>
    <div class="jumbo">
        <figure>
            <img src="../assets/img/jumbotron.jpg" alt="">
        </figure>
        <div>
            <p>Current series</p>
        </div>
    </div>
    <div class="container">
        <div v-for="(book, index) in books" :key="index">
            <figure>
                <img :src="book.thumb" :alt="book.series">
                <span>{{ book.series }}</span>
            </figure>
            
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

    .jumbo{
        position: relative;
        figure{
            height: 700px;

            img{
                height: 100%;
                width: 100%;
                object-fit: cover;
                object-position: top;
                display: block;
            }
        }

        div{
            display: flex;
            align-items: center;
            position: absolute;
            bottom: -20px;
            left: 10%;
            p{
                text-transform: uppercase;
                background-color:#0282f9;
                -webkit-box-shadow: 5px 5px 10px 5px #000000; 
                box-shadow: 5px 5px 10px 5px #000000;
                padding: 20px;
                font-size: 30px;
                font-weight: bold;
                color: #ffffff;
            }
        }
    }

    .container{
        width: 100%;
        background-color: #1c1c1c;
        padding-block: 50px;

        div{
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            width: 80%;
            margin: 0 auto;
            figure{
                width: calc(100% / 6 - 30px);
                height: 400px;
                img{
                    width: 100%;
                    height: 100%;
                    object-fit: cover;
                    object-position: top;
                    display: block;
                }
            }
        }
    }
    

</style>