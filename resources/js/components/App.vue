<template>

    <nav class="header-menu">

        <ul class="header-menu__list">

            <li class="header-menu__item">
                <a href="#">Menu item 1</a>
            </li>

            <li class="header-menu__item">
                <a href="#">Menu item 2</a>
            </li>

            <li class="header-menu__item">
                <a href="#">Menu item 3</a>
            </li>

        </ul>

    </nav>

</template>

<script>
    export default {
        name: "App"
    }
</script>

<style lang="scss" scoped>

    @import "../../sass/variables";

    nav.header-menu {
        background-color: greenyellow;
        height: 50px;

        ul.header-menu__list {
            margin: 0;
            padding: 0;
            height: 100%;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;

            li.header-menu__item {
                list-style: none;
                a {
                    text-decoration: none;
                    color: black;
                    &:hover {
                        color: red;
                    }
                }
            }
        }

        @media screen and (max-width: $laptopScreen){
            background-color: yellow;
        }

        @media screen and (max-width: $tabletScreen){
            background-color: yellowgreen;
        }

        @media screen and (max-width: $mobileScreen){
            background-color: red;
        }

    }

</style>
