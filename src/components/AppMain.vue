<script>
export default{
    data (){
        return{
            
        }
    }
}

</script>

<template>
<main>
    <div class="container-main">
        <h2> -> Content goes here <- </h2>
    </div>
</main>
</template>


<style scoped lang="scss">

@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

main{
    background-color: black;
    height: 200px;
    width: 100%;
    @include flex (row, left, center);
}
.container-main{
    width: 50%;
    @include flex (row, left, center);

    h2{
        color: white;
        margin: auto;
    }
}
</style>