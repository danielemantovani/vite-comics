<script>
export default {
    data() {
        return {

        }
    }
}

</script>

<template>
    <footer>
        <div class="container-footer">
            <div class="left-col">

            </div>
            <div class="right-col">
                <img src="/src/assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </footer>

</template>


<style scoped lang="scss">

@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

    footer{
        background-image: url(../assets/img/footer-bg.jpg);
        height: 25rem;
    }

    .container-footer{
        width: 70%;
        margin: auto;
        
        .right-col{
            @include flex(row, right, center);
            img{
                width: 25rem;
            }
        }
    }

</style>