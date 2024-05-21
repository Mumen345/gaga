<template>
<div class="hero_banner">
    <div class="div_left">
        <div class="left_nav">
            <h5>LOGO</h5>
        </div>
        <h1>CREATE. <br> CONNECT. <br> CONQUER.</h1>
        <button @click="openCreative" class="secondarybtn"> Get Started</button>
        <div class="img_div">
            <img class="lit_image" src="../assets/images/first.png" alt="">
            <img class="little_images" src="../assets/images/second.png" alt="">
            <img class="little_images" src="../assets/images/third.png" alt="">
        </div>
    </div>
    <div class="div_right">
        <NavigationBar />
        <h1>Where Brands Meet Culture</h1>
        <button class="secondarybtn"> Get Started</button>

    </div>
</div>
</template>

<script>
import NavigationBar from './NavigationBar.vue';
export default {
    components: {
        NavigationBar
    },
    methods: {
        openCreative() {
            this.$router.push('/creative')
        }

    }
}
</script>

<style scoped>
.hero_banner {
    display: flex;
    flex-direction: row;
    width: 100%;
}

.div_left {
    background-image: url("../assets/images/left.png");
    display: flex;
    flex-direction: column;
    padding-bottom: 10rem;
    justify-content: space-between;
    align-items: center;
    background-color: #0A2D4E;
    height: 100vh;
    box-sizing: border-box;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    width: 50%;
    font-family: archivo;
    font-size: 3rem;
    text-align: center;
    color: #ffffff !important;
    text-transform: capitalize !important;
}

.div_right h1 {
    font-size: 5.5rem;
    text-align: center;

}

h5 {
    font-size: 2rem;
}

.div_right {
    width: 50%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding-bottom: 10rem;
    align-items: center;
    background-image: url("../assets/images/right.png");
    height: 100vh;
    box-sizing: border-box;
    background-position: center;
    background-repeat: no-repeat;
    color: #ffffff;
    background-size: cover;
    font-family: archivo;
}

.little_images {
    margin-left: -4.5rem;
    box-sizing: border-box;
}

.img_div {
    margin: 20px auto;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.left_nav {
    background: #E9E9FF;
    width: 100%;
    height: 103px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #000000;
}

.right_nav p {
    color: none;
    font-family: BrinnanRegular;
    font-size: small;
}

.right_nav {
    background: none;
    width: 100%;
    height: 103px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    border-bottom: 1px solid #C2C2C2;

}

@media only screen and (max-width: 1366px) {
    .div_left {
        font-size: 2.3rem;
    }

    .lit_image {
        width: 10rem !important;
    }

    .little_images {
        margin-top: 20px;
        margin-left: -3.5rem;
        box-sizing: border-box;
        width: 10rem !important;
    }

    .div_right h1 {
        font-size: 4.5rem;

    }
}

@media only screen and (max-width: 1900px) {
    .lit_image {
        width: 8rem !important;
    }
    
    .little_images {
        margin-top: 20px;
        margin-left: -3.5rem;
        box-sizing: border-box;
        width: 8rem !important;
    }
    .div_right h1 {
    font-size: 2.9rem !important;
    text-align: center;

}
.div_left {
        font-size: 1.7rem;
    }
}

@media only screen and (max-width: 1095px) {
    .hero_banner {
        display: flex;
        flex-direction: column-reverse;
        width: 100%;
        height: auto;
    }

    .div_right {
        width: 100%;
        display: flex;
        height: 70vh;

    }

    .div_left {
        width: 100%;
        display: flex;
        height: auto;
    }
}

@media only screen and (max-width: 600px) {
    .div_right h1 {
        font-size: 2.8rem;

    }

    .lit_image {
        width: 8rem !important;
    }

    .little_images {
        margin-left: -2.5rem;
        box-sizing: border-box;
        width: 8rem !important;
    }
}
</style>
