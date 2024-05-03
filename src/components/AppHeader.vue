<script>
export default {
    data() {
        return {
            menu: [
                {
                    section: "CHARACTERS",
                    isVisible: false,
                },
                {
                    section: "COMICS",
                    isVisible: true,
                },
                {
                    section: "MOVIES",
                    isVisible: false,
                },
                {
                    section: "TV",
                    isVisible: false,
                },
                {
                    section: "GAMES",
                    isVisible: false,
                },
                {
                    section: "COLLECTIBLES",
                    isVisible: false,
                },
                {
                    section: "VIDEOS",
                    isVisible: false,
                },
                {
                    section: "FANS",
                    isVisible: false,
                },
                {
                    section: "NEWS",
                    isVisible: false,
                },
                {
                    section: "SHOP",
                    isVisible: false,
                },
            ]
        }
    }
}

</script>

<template>
    <header>
        <div class="header-container">
            <div>
                <img src="/src/assets/img/dc-logo.png" alt="Logo DC Comics">
            </div>
            <ul class="menu">
                <li v-for="curItem in menu">
                    <a href="" :class="{active : curItem.isVisible}">{{ curItem.section }}</a>
                </li>
            </ul>
        </div>

    </header>

</template>


<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.header-container {
    @include flex(row, space-between, center);
    width: 70%;
    margin: 20px auto;
}

.menu {
    @include flex(row, center, center);
}

ul {
    list-style-type: none;

    a {
        text-decoration: none;
        color: black;
        margin-right: .8rem;
        font-size: 0.8rem;
        font-weight: bolder;

        &:hover {
            color: $primary-color;
        }
        
        &.active {
            border-bottom: 5px solid $primary-color;
        }
    }

}
</style>