<script>
export default {
  data() {
    return {
        footerItems: [
            {
          title: "DC COMICS",
          list: ["Charaters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
        },
        {
          title: "SHOP",
          list: ["Shop DC", "Shop DC Collectibles"]
        },
        {
          title: "DC",
          list: ["Terms Of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificates", "Rating", "Shop Help", "Contact Us"]
        },
        {
          title: "SITES",
          list: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"]
        },
      ], 
      
    };
  },
};
</script>

<template>
    <div class="background ">
        <div class="container list">
            <div v-for="item in footerItems">
                <h4 class="list-title">{{ item.title }}</h4>
                <ul>
                    <li v-for="item in item.list"><a href="">{{ item }}</a></li>
                </ul>
            </div>
            <div class="dc-logo"></div>
        </div>
        
    </div>

</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;
.background{
    background-image: url(../assets/img/footer-bg.jpg) ;
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    height: 300px;    
}

.list {    
    display: flex;
    gap: 1rem;
}
.list-title{
    color: white;
    margin-top: 2rem;
}

a {
    color: white;
    text-decoration: none;
    font-size: 0.5rem;
}

li {
    list-style-type: none;
}

.dc-logo {
    background-position: center;
    background-repeat: no-repeat;
    background-size: 450px;
    background-image: url(../assets/img/dc-logo-bg.png);
    width: 50%;
    height: 300px; 
    margin-left: auto;
    
       
  }

</style>