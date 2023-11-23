<script>
export default {
  data() {
    return {
      navItems: [
        {
          title: "CHARACTERS",          
        },
        {
          title: "COMICS",      
        },
        {
          title: "MOVIES",          
        },
        {
          title: "TV",          
        },
        {
          title: "GAMES",          
        },
        {
          title: "COLLECTIBLES",      
        },
        {
          title: "VIDEOS",          
        },
        {
          title: "FANS",          
        },
        {
          title: "NEWS",          
        },
        {
          title: "SHOP",      
        },        
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="DC" />
    </div>
    <nav>
      <ul>
        <li v-for="item in navItems" >
          <a href="">{{ item.title }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

img {
    width: 70px;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: white;
}

ul{
    display: flex;
    gap: 1rem;
}

a {
    text-decoration: none;
    color: black;
    font-size: 0.7rem;
    height: 100px;
    display: flex;
    align-items: center;
    &:hover {
        border-bottom: 4px solid $primary ;
        color: $primary;
    }
}

li {
    list-style: none;
    
}

</style>