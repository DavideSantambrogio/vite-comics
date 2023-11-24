<script>
export default {
    props: {
        thumb: String,
        series: String
    },
    computed: {
    uppercaseSeries() {      
      return this.series.toUpperCase();
    }  
    }
}

</script>

<template>
    <div>
        <img :src="thumb" alt="">
        <p>{{ uppercaseSeries }}</p>
    </div>

</template>

<style lang="scss" scoped>
img{
    width: 150px;
    height: 170px;
    object-fit: cover;
    object-position: top;
}

p {
    width: 110px;
    font-size: .8rem;
}





</style>