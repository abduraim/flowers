<template>

    <div class="wrapper">
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
    </div>

</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style lang="scss" scoped>

    @import "../../../sass/variables";
    @import "../../../sass/media_queries_mixins";

    nav.header-menu {
        height: $headerHeight;
        width: 100%;
        position: fixed;
        top: 0;
        left: 0;
        background-color: greenyellow;

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

        @include landscape {
            height: 100%;
            width: $headerHeight;

            ul.header-menu__list {
                flex-direction: column;
            }
        }

    }

</style>
