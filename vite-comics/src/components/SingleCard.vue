<script>

    export default{
        name: "SingleCard",
        props:{
            propsSrc: String,
            propsSeries: String
        },
    }

</script>

<template>

    <figure>
        <img :src="propsSrc" :alt="propsSeries">
        <h4>{{ propsSeries }}</h4>
    </figure>

</template>

<style scoped lang="scss">

    figure{
        display: flex;
        flex-direction: column;
        width: calc(100% / 6 - 50px);

        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
            display: block;
            

            &:hover{
                transform: scale(1.1);
                cursor: pointer;
                -webkit-box-shadow: 1px 1px 20px 5px #0282f9; 
                box-shadow: 1px 1px 20px 5px #0282f9;
            }
        }
        h4{
            color: #fff;
            margin-top: 30px;
            text-align: center;
            text-transform: uppercase;
            
        }
    }
</style>