<script>
export default {
  data() {
    return {
        socialList: [
        {
            icon: "../src/assets/img/footer-facebook.png",
            name: "facebook",
            link: "www.facebook.com"
        },
        {
            icon: "../src/assets/img/footer-twitter.png",
            name: "twitter",
            link: "www.twitter.com"
        },
        {
            icon: "../src/assets/img/footer-youtube.png",
            name: "youtube",
            link: "www.youtube.com"
        },
        {
            icon: "../src/assets/img/footer-pinterest.png",
            name: "pinterest",
            link: "www.pinterest.com"
        },
        {
            icon: "../src/assets/img/footer-periscope.png",
            name: "periscope",
            link: "www.periscope.com"
        }
      ]
      
    };
  },
};
</script>

<template>
    <section>
        <div class="container social">
            <button>SIGN-UP NOW!</button>
            <div class="social-list">
                <h3>FOLLOW US</h3>
                <ul>
                    <li v-for="social in socialList">
                    <a :href="`http://${social.link}`"><img :src=(social.icon) :alt="`${social.name}`"></a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

section {
    background-color: #282828;
}
.social {
    display: flex;
    align-items: center;
    padding: 2rem;
    justify-content: space-between;
}
.social-list {
    display: flex;
    align-items: center;
    gap: 1rem;
}

h3 {
    color: $primary;
}

ul {
    display: flex;
    gap: 1rem;
    list-style-type: none;
}

a {
    text-decoration: none;
}

button {
    background-color: inherit;
    border: 2px solid $primary;
    padding: 0.7rem;
    color: white;

}



</style>