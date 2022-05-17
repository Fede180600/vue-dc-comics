<template>
    <header class="header">
        <div class="container">
            <div class="header_logo">
                <img src="../assets/img/dc-logo.png" alt="Logo DC Comics">
            </div>
            <nav>
                <ul class="header_menu">
                    <li v-for="(link, index) in links" :key="index"><a href="" :class="{ active: link.active }">{{ link.text }}</a></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: "AppHeader",
    data: function() {
        return{
            links: [
                {
                    url: "#",
                    text: "characters",
                    active: false,
                },
                {
                    url: "#",
                    text: "comics",
                    active: true,
                },
                {
                    url: "#",
                    text: "movies",
                    active: false,
                },
                {
                    url: "#",
                    text: "tv",
                    active: false,
                },
                {
                    url: "#",
                    text: "games",
                    active: false,
                },
                {
                    url: "#",
                    text: "collectibles",
                    active: false,
                },
                {
                    url: "#",
                    text: "videos",
                    active: false,
                },
                {
                    url: "#",
                    text: "fans",
                    active: false,
                },
                {
                    url: "#",
                    text: "news",
                    active: false,
                },
                {
                    url: "#",
                    text: "shop",
                    active: false,
                },

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";
.header{
    height: 80px;
    .container{
        height: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    &_logo{
        width: 50px;
    }
    &_menu{
        text-transform: uppercase;
        height: 100%;
        li {
            display: inline-block;
            margin: 0 20px;

            a{
                color: $brand-secondary-color;
                font-size: 12px;
                font-weight: 500;
                line-height: 80px;
                padding-bottom: 28px;
                border-bottom: 5px solid transparent;
                &.active {
                    color: $brand-primary-color;
                    border-bottom: 5px solid $brand-primary-color;
                    color: $brand-primary-color;
                }
            }
        }

    }
}
</style>
    
