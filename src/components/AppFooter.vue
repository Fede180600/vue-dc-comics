<template>
    <footer class="footer">

        <div class="footer_top">
            <div class="container">
                <div class="col_text"></div>
                <div class="col_logo">
                </div>
            </div>
        </div>
        <div class="footer_bottom">
            <div class="container">
                <div class="col_btn">
                    <button>sing-up now!</button>
                </div> 
                <div class="col_socials">
                    <span>follow us</span>
                    <ul class="socials">
                        <li v-for="(social, index) in socials" :key="index">
                            <img :src="require(`../assets/img/${social.logoSrc}`)" alt="">
                        </li>
                    </ul>
                </div>
            </div>
        </div>

    </footer>
</template>
<script>
export default {
    name: "AppFooter",
    data: function() {
        return {
            socials: [
                {
                    logoSrc: "footer-facebook.png"
                },
                {
                    logoSrc: "footer-periscope.png"
                },
                {
                    logoSrc: "footer-pinterest.png"
                },
                {
                    logoSrc: "footer-twitter.png"
                },
                {
                    logoSrc: "footer-youtube.png"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped >
@import "../style/variables.scss";

.footer {
    // height: 470px;
    background-color: $brand-secondary-color;

    &_top {
        height: 400px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        .container {
            display: flex;
            justify-content: space-between;
        }
        .col_text {
            width: 40%;
        }
        .col_logo {
            width: 40%;
            height: 400px;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-position: center;
            background-size: cover;
        }
    }

    &_bottom {
        height: 70px;
        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            button {
                padding: 10px;
                text-transform: uppercase;
                background-color: transparent;
                color: white;
                border: 1px solid $brand-primary-color;
            }

            .col_socials {
                height: 100%;
                display: flex;
                align-items: center;
                span {
                    text-transform: uppercase;
                    color: $brand-primary-color;
                    font-weight: 600;
                }
                .socials {
                    margin-left: 20px;
                    li {
                        display: inline-block;
                        margin: 0 10px;
                        img {
                            height: 30px;
                        }
                    }
                }
            }
        }
    }
}
</style>