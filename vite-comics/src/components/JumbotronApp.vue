<script>
import ListBooksApp from './ListBooksApp.vue';

export default {
  name: "JumbotronApp",
  components:{
    ListBooksApp,
  },
}
</script>

<template>
    <div class="jumbo">
        <figure>
            <img src="../assets/img/jumbotron.jpg" alt="">
        </figure>
        <div class="series">
            <p>Current series</p>
        </div>
    </div>

    <ListBooksApp/>
</template>

<style scoped lang="scss">
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

        .series{
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
</style>