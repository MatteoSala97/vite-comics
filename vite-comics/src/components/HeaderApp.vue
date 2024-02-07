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
  justify-content: space-between;

  figure{
    
    img{
      width: 100%;
    }
  }
}

ul{

  display: flex;
  gap: 10px;
  align-items: center;

  li{
    list-style-type: none;
    
    a{
      text-transform: uppercase;
      text-decoration: none;
      color: $font-color-main;
    }
  }
}
</style>
