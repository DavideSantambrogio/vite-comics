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



</style>