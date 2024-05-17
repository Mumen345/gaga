<template>
    <div class="hero_div">
        <img class="img_responsive" src="../assets/images/right_image.png" alt="">
        <div>
            <NavigationBar />
            <div class="right_text">
                <h1 class="">We craft compelling <span>content</span> to fuel your brand growth</h1>
                <p class="">Generating various forms of creative content tailored to you solely to achieve your
                    specific goal.
                </p>
                <a href="#" class="hero_btn">
                    Schedule Meeting
                    <img src="../assets/images/right_arrow.svg" alt="">
                </a>
            </div>
        </div>
    </div>
</template>

<script>
import NavigationBar from './NavigationBar.vue';

export default {
    components: {
        NavigationBar
    }
}
</script>

<style scoped>
.hero_div img {
    z-index: 100 !important;
    /* width: 100%; */
}

.hero_div {
    display: flex;
    width: 100%;
    flex-direction: row;
    background-image: url("../assets/images/hero_bg.svg");
    background-repeat: no-repeat;
    background-position: center;
    background-color: #ffffff;
    justify-content: center;
    align-items: start;
}

.right_text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 20px;
    text-align: center;
}

.right_text p {
    font-size: 18px;
    font-weight: 300;
    line-height: 21px;
    letter-spacing: 0em;
    text-align: center;
    width: 50%;
    margin: -50px 0 auto;
    color: #676767;
    font-family: BrinnanLight;
}

h1 {
    font-size: clamp(5.4rem, 10vw, 2rem);
    font-weight: 900;
    font-family: 'ReportFont';
    color: #2A2929;
}

.hero_btn {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #FF540B;
    padding: 20px;
    width: 264px;
    border-radius: 45px;
    gap: 15px;
    font-size: 20px;
    color: #ffffff;

}


/* Resoponsiveness */

@media only screen and (max-width: 1295px) {
    .right_text p {
        width: 90%;
        margin: -40px 0 auto;
        color: #676767;
        font-family: BrinnanLight;
    }

    h1 {
        font-size: clamp(4.5rem, 10vw, 2rem);
        line-height: 70px;
        font-weight: 900;
        font-family: 'ReportFont', cursive;
        color: #2A2929;
    }
}

@media only screen and (max-width: 1116px) {
    .hero_div {
        display: flex;
        width: 100%;
        flex-direction: column-reverse;
        gap: 30px;
        justify-content: center !important;
        align-items: center !important;
        background-image: url("../assets/images/hero_bg.svg");
        background-repeat: no-repeat;
        background-position: center;
        background-color: #ffffff;
    }

    .img_responsive {
        width: 100%;
    }
}

@media only screen and (max-width: 578px) {
    h1 {
        font-size: clamp(3.5rem, 5vw, 1rem) !important;
        line-height: 55px;
        font-weight: 900;
        font-family: 'ReportFont';
        color: #2A2929;
    }

    .hero_btn {
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #FF540B;
        padding: 20px;
        width: 234px;
        border-radius: 45px;
        gap: 15px;
        font-size: 20px;
        color: #ffffff;

    }
}
</style>