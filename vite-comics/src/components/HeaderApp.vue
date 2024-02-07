<script>

export default {
  name: "HeaderApp",
};
</script>

<template>
 <div>
  <figure>
    <img src="../assets/img/dc-logo.png" alt="">
  </figure>
  <div>
    <ul>
      <li>
        <a href="#">characters</a>
      </li>
      <li>
        <a href="#">comics</a>
      </li>
      <li>
        <a href="#">movies</a>
      </li>
      <li>
        <a href="#">tv</a>
      </li>
      <li>
        <a href="#">games</a>
      </li>
      <li>
        <a href="#">collectibles</a>
      </li>
      <li>
        <a href="#">videos</a>
      </li>
      <li>
        <a href="#">fans</a>
      </li>
      <li>
        <a href="#">news</a>
      </li>
      <li>
        <a href="#">shop</a>
      </li>
    </ul>
  </div>
 </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "../styles/partials/mixins" as *;

div{
  display: flex;
  justify-content: space-around;
  margin: 20px 0;

  figure{
    
    img{
      width: 100%;
    }
  }

  div{
    ul{
    
      display: flex;
      gap: 30px;
      align-items: center;
    
      li{
        list-style-type: none;
        font-weight: bold;
    
        a{
          text-transform: uppercase;
          text-decoration: none;
          color: $font-color-main;
          padding-block: 40px;

          &:hover{
            color: blue;
            border-bottom: 5px solid blue;
          }
        }
      }
    }
  }
}

</style>
