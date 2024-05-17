<template>
    <div class="footer_container">
        <div class="first_image">
            <img src="../assets/images/Line10.svg" alt="">
            <img src="../assets/images/Vector.svg" alt="">
            <img src="../assets/images/Line11.svg" alt="">
        </div>
        <p class="header">
            LET'S DISCUSS<br /> YOUR BRAND
        </p>

        <div class="social_media">
            <img src="../assets/images/instagram.svg" alt="">
            <img src="../assets/images/facebook.svg" alt="">
            <img src="../assets/images/twitter.svg" alt="">
            <img src="../assets/images/youtube.svg" alt="">
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer_container {
    background-color: #FF540B;
    height: 688px;
    width: 90%;
    margin: 40px auto;
    border-radius: 0px 0px 120px 120px !important;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    padding: 50px 0;
}

.first_image {
    display: flex;
    justify-content: center;
    align-items: center;
}

.header {
    font-family: ReportFont;
    font-size: 105px;
    font-weight: 900;
    line-height: 126px;
    letter-spacing: 0em;
    text-align: center;
    color: #ffffff;

}

.social_media {
    display: flex;
    gap: 20px;
    justify-content: center;
    align-items: center;
}

.hover_div {
    /* display: none; */
}

@media only screen and (max-width: 1298px) {
    .footer_container {
        background-color: #FF540B;
        height: 400px;
        width: 95%;
        margin: 0 auto;
        border-radius: 0px 0px 120px 120px !important;
    }
}

@media only screen and (max-width: 1100px) {
    .footer_container {
        background-color: #FF540B;
        height: 400px;
        width: 95%;
        margin: 0 auto;
        border-radius: 0 !important;
    }

    .header {
        font-family: ReportFont;
        font-size: 75px;
        font-weight: 900;
        line-height: 86px;
        letter-spacing: 0em;
        text-align: center;
        color: #ffffff;

    }

    .social_media {
        display: flex;
        gap: 40px;
        justify-content: center;
        align-items: center;
        width: 100%;
    }

    .first_image {
        display: none;
    }

    @media only screen and (max-width: 500px) {
        .header {
            font-family: ReportFont;
            font-size: 35px;
            font-weight: 900;
            line-height: 66px;
            letter-spacing: 0em;
            text-align: center;
            color: #ffffff;

        }

        .social_media {
            display: flex;
            gap: 10px;
            justify-content: center;
            align-items: center;
            width: 100%;
        }

        .footer_container {
            background-color: #FF540B;
            height: 400px;
            width: 100%;
            margin: 0 auto;
            border-radius: 0 !important;
        }
    }


}
</style>