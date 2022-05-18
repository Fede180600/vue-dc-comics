<template>
    <section class="blue-line">
        <div class="container">
            <ul class="icons-list">
                <li v-for="(item, index) in icons" :key="index">
                    <img :src="require(`../assets/img/${item.img}`)" alt="">
                    <h3>{{ item.text }}</h3>
                </li>
            </ul>
        </div>
    </section>
</template>
<script>
export default {
    name: "AppBlueLine",
    data: function() {
        return {
            icons: [
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'Subscription'
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'Comic Shop Locator'
                },
                {
                    img: 'buy-dc-power-visa.svg',
                    text: 'DC power visa'
                }
            ]
        }
    }
}
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
.blue-line{
    padding: 60px;
    background-color: $brand-primary-color;
    .container {
        height: 100%;
        .icons-list {
            display: flex;
            align-items: center;
            height: 100%;
            li {
                width: calc(100% / 5);
                color: white;
                display: flex;
                align-items: center;
                img {
                    max-width: 45px;
                    max-height: 45px;
                    object-fit: contain;
                    margin-right: 10px;
                }
                h3 {
                    font-weight: 400;
                    text-transform: uppercase;
                    font-size: 14px;;
                }
            }
        }
    }
}
</style>