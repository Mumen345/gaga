<template>
<div class="creative_hero">
    <div class="top_div">
        <img class="lit_image" src="../assets/images/Ellipse.png" alt="">
        <img class="little_images" src="../assets/images/Ellipse2.png" alt="">
        <img class="little_images" src="../assets/images/Ellipse3.png" alt="">
    </div>
    <div class="bottom_div">
        <h1>CREATE. CONNECT. CONQUER.</h1>
        <p>We Help Creators Grow whilst maintaining consistency and quality. Experience Premier Talent Management and Creative Support with Gaaga Agency.</p>
        <button class="secondarybtn">Get Started</button>
    </div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.creative_hero {
    background-image: url("../assets/images/left.png");
    box-sizing: border-box;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    height: 100%;
    padding: 5rem 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 70px;

}

.creative_hero p {
    font-size: 16px;
    color: #fff;
    width: 640px;
    line-height: 25px;
}

.creative_hero h1 {
    color: #fff;
    font-size: 48px;
    font-family: archivo;
    line-height: 0;
    margin: 0;
}

.bottom_div {
    display: flex;
    gap: 30px;
    flex-direction: column;
    text-align: center;
    justify-content: center;
    align-items: center;
}

.little_images {
    margin-left: -4.5rem;
    box-sizing: border-box;
}

@media only screen and (max-width: 1366px) {

    .lit_image {
        width: 25rem !important;
    }

    .little_images {
        margin-top: 20px;
        width: 25rem !important;
        margin-left: -3.5rem;
        box-sizing: border-box;
    }
}

@media only screen and (max-width: 1132px) {
    .lit_image {
        width: 20rem !important;
    }

    .little_images {
        margin-top: 20px;
        margin-left: -3.5rem;
        box-sizing: border-box;
        width: 20rem !important;
    }
}

@media only screen and (max-width: 1095px) {
    .lit_image {
        width: 18rem !important;
    }

    .little_images {
        margin-top: 20px;
        margin-left: -3.5rem;
        box-sizing: border-box;
        width: 18rem !important;
    }
    
    .creative_hero h1 {
        color: #fff;
        font-size: 48px;
        font-family: archivo;
        line-height: 50px;
        margin: 0;
    }
    
    .bottom_div {
        display: flex;
        gap: 30px;
        flex-direction: column;
        text-align: center;
        justify-content: center;
        align-items: center;
    }
    
    .creative_hero p {
        font-size: 16px;
        color: #fff;
        width: 80%;
        margin: 0 auto;
        
    }
    
    @media only screen and (max-width: 779px) {
        .lit_image {
            width: 14rem !important;
        }
        
        .little_images {
            margin-top: 0;
            margin-left: -3.5rem;
            box-sizing: border-box;
            width: 14rem !important;
        }
    }
    @media only screen and (max-width: 590px) {
        .lit_image {
            width: 10rem !important;
        }
        
        .little_images {
            margin-top: 0;
            margin-left: -3.5rem;
            box-sizing: border-box;
            width: 10rem !important;
        }
        .top_div {
            width: 90% !important;
            margin: 0 auto !important;
            display: flex;
            justify-content: center;
            align-items: center;
        }
    }.creative_hero {
        gap: 40px;
    }
    @media only screen and (max-width: 320px) {
        .lit_image {
            width: 8rem !important;
        }
        
        .little_images {
            margin-top: 0;
            margin-left: -3.5rem;
            box-sizing: border-box;
            width: 8rem !important;
        }
    }
}
</style>
