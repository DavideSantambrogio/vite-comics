<script>
export default {
  data() {
    return {
        callToActList: [
        {
          icon: "../src/assets/img/buy-comics-digital-comics.png",
          name: "DIGITAL COMICS",            
        },
        {
          icon: "../src/assets/img/buy-comics-merchandise.png",
          name: "DC MERCHANDISE",            
        },
        {
          icon: "../src/assets/img/buy-comics-subscriptions.png",
          name: "SUBSCRITION",            
        },
        {
          icon: "../src/assets/img/buy-comics-shop-locator.png",
          name: "COMICS SHOP LOCATOR",            
        },
        {
          icon: "../src/assets/img/buy-dc-power-visa.svg",
          name: "DC POWER VISA",            
        }
      ]
      
    };
  },
};
</script>

<template>
    <section>
        <div class="container"> 
          <ul>
            <li v-for="callToAct in callToActList">
              <img :src=(callToAct.icon) :alt="`${callToAct.name}`">
              <p>{{callToAct.name}}</p>
            </li>
          </ul>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

section {
  background-color: $primary;
}

li:last-child img{
  width: 3rem;
}

img {
   
  height: 3rem;
}

ul {
  display: flex;
  align-items: center;
  padding: 2rem;
  justify-content: space-around;
}

li {
  list-style-type: none;
  display: flex;
  color: white;
  align-items: center;
  gap: 0.5rem;
  
}

p {
  font-size: 0.7rem;
}

</style>

