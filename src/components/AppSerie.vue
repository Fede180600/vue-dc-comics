<template>
    <div class="serie_box">
        <div class="serie_img">
            <img :src="productObj.thumb" alt="">
        </div>
        <div class="serie_description_text">
            <h4>{{ productObj.series }}</h4>
            <span>{{ productObj.price }}</span>
            <br>
            <small>{{ productObj.type }}</small>
        </div>
    </div>
</template>

<script>
export default {
    name: "AppSerie",
    props: {
        productObj: Object,
    }
}
</script>

<style lang="scss">
.serie_box {
    width: calc(100% / 6 - 20px);
    margin: 10px;
    display: flex;
    flex-direction: column;
    .serie_img {   
        width: 100%;
        height: 0;
        padding-bottom: 100%;
        object-fit: cover;
        object-position: top;
        overflow: hidden;
        margin-bottom: 10px;
    }
    .serie_description_text {
        text-transform: uppercase;
        h4 {
            font-weight: 400;
            font-size: 14px;
        }
        span {
            font-size: 12px;
        }
        small {
            font-size: 10px;
        }
    }
}
</style>