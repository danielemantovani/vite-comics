<script>

export default {
    props: {
        cardImage: String,
        cardTitle: String
    }
}

</script>

<template>
    <div class="card">
        <img :src="cardImage" :alt="cardTitle" />
        <h4>{{cardTitle}}</h4>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin.scss" as *;

    .card{
        
        img{
            height: 250px;
            
        }
        h4{
            color: white;
            text-align: center;
        }
    }

</style>