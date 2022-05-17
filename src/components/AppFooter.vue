<template>
    <footer class="footer">

        <div class="footer_top">
            <div class="container">
                <div class="col_text"></div>
                <div class="col_logo">
                    <!-- <img src="../assets/img/dc-logo-bg.png" alt=""> -->
                </div>
            </div>
        </div>
        <div class="footer_bottom">
            <div class="container">
                footer bottom 
            </div>
        </div>

    </footer>
</template>
<script>
export default {
    name: "AppFooter"

}
</script>
<style lang="scss" scoped >
@import "../style/variables.scss";

.footer {
    height: 470px;
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
    }
}
</style>