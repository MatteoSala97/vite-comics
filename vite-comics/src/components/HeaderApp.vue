<script>

export default {
  name: "HeaderApp",
  data(){
    return {
      menuLinks: [
        {
          name: "characters",
          link: "#",
          current: false
        },
        {
          name: "comics",
          link: "#",
          current: true
        },
        {
          name: "movies",
          link: "#",
          current: false
        },
        {
          name: "tv",
          link: "#",
          current: false
        },
        {
          name: "games",
          link: "#",
          current: false
        },
        {
          name: "collectibles",
          link: "#",
          current: false
        },
        {
          name: "videos",
          link: "#",
          current: false
        },
        {
          name: "fans",
          link: "#",
          current: false
        },
        {
          name: "news",
          link: "#",
          current: false
        },
        {
          name: "shop",
          link: "#",
          current: false
        },
      ]
    }
  }
};
</script>

<template>
  <div>
    <figure>
      <a href="#">
        <img src="../assets/img/dc-logo.png" alt="Dc Logo">
      </a>
    </figure>
    <ul>
      <li v-for="(element, index) in menuLinks" :key="index">
        <a :class="element.current ? 'active' : '' " href="#">{{ element.name }}</a>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *; 
@use "../styles/partials/mixins" as *; 

div{
  display: flex;
  justify-content: space-around;
  margin: 20px auto;

  figure{
    
    img{
      width: 100%;
    }
  }

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
        color: black;
        padding-block: 58px;

        &:hover{
          color: #0282f9;
          border-bottom: 5px solid #0282f9;
        }
      }
    }
  }
}
.active{
  color: #0282f9;
  border-bottom: 5px solid #0282f9;
}
</style>
