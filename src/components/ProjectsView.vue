<template>
    <div class="project_container">
        <p class="little_header">PROJECTS <span><img src="../assets/images/long_arrow.svg" alt="arrow"></span> </p>
        <div class="project_images">
            <div class="img_row">
                <div class="container">
                    <img class="main_img " src="../assets/images/first.png" alt="">
                    <div class="t">
                        <img src="../assets/images/hover_arrow.svg" alt="">
                        <!-- <p class="artist_year">2023</p> -->
                        <p class="artist_name">Artist Name</p>
                    </div>
                </div>
                <div class="container">
                    <img class="main_img" src="../assets/images/second.png" alt="">
                    <div class="t">
                        <img src="../assets/images/hover_arrow.svg" alt="">
                        <!-- <p class="artist_year">2023</p> -->
                        <p class="artist_name">Artist Name</p>
                    </div>
                </div>
            </div>
            <div class="img_row">
                <div class="container">
                    <img class="main_img" src="../assets/images/three.png" alt="">
                    <div class="t">
                        <img src="../assets/images/hover_arrow.svg" alt="">
                        <!-- <p class="artist_year">2023</p> -->
                        <p class="artist_name">Artist Name</p>
                    </div>
                </div>
                <div class="container">
                    <img class="main_img" src="../assets/images/forth.png" alt="">
                    <div class="t">
                        <img src="../assets/images/hover_arrow.svg" alt="">
                        <!-- <p class="artist_year">2023</p> -->
                        <p class="artist_name">Artist Name</p>
                    </div>
                </div>
            </div>

            <div class="img_row">
                <div class="container">
                    <img class="main_img" src="../assets/images/fifth.png" alt="">
                    <div class="t">
                        <img src="../assets/images/hover_arrow.svg" alt="">
                        <!-- <p class="artist_year">2023</p> -->
                        <p class="artist_name">Artist Name</p>
                    </div>
                </div>
                <div class="container">
                    <img src="../assets/images/sixth.png" alt="" />
                    <div class="t">
                        <img src="../assets/images/hover_arrow.svg" alt="">
                        <!-- <p class="artist_year">2023</p> -->
                        <p class="artist_name">Artist Name</p>
                    </div>
                </div>

            </div>
        </div>
        <div class="mobile_friendly">


            <div class="img_row">
                <div class="image_wrapper">
                    <img src="../assets/images/first.png" alt="" />
                    <div class="overlay overlay_1">
                        <h3>Artist Name</h3>
                        <P>2023</P>
                    </div>
                </div>
                <div class="image_wrapper">
                    <img src="../assets/images/second.png" alt="" />
                    <div class="overlay overlay_1">
                        <h3>Artist Name</h3>
                        <P>2023</P>
                    </div>
                </div>
            </div>
            <div class="img_row">
                <div class="image_wrapper">
                    <img src="../assets/images/three.png" alt="" />
                    <div class="overlay overlay_1">
                        <h3>Artist Name</h3>
                        <P>2023</P>
                    </div>
                </div>
                <div class="image_wrapper">
                    <img src="../assets/images/forth.png" alt="" />
                    <div class="overlay overlay_1">
                        <h3>Artist Name</h3>
                        <P>2023</P>
                    </div>
                </div>
            </div>
            <div class="img_row">
                <div class="image_wrapper">
                    <img src="../assets/images/fifth.png" alt="" />
                    <div class="overlay overlay_1">
                        <h3>Artist Name</h3>
                        <P>2023</P>
                    </div>
                </div>
                <div class="image_wrapper">
                    <img src="../assets/images/sixth.png" alt="" />
                    <div class="overlay overlay_1">
                        <h3>Artist Name</h3>
                        <P>2023</P>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.overlay {
    position: absolute;
    background: #00000099;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #ffffff;
}

.overlay_1 p {
    font-family: BrinnanBold;

}

.overlay_1 h3 {
    font-family: BrinnanBold;
    font-size: 20px;
}

.overlay_1 {
    left: 0;
    bottom: 3px;
    width: 100%;
    border-radius: 0 0 30px 30px;

}

.image_wrapper img {
    width: 100%;
    border-radius: 30px;
}

.image_wrapper {
    position: relative;
    width: 100%;
}

.image_wrapper:hover .overlay_3 {
    transform: scale(1);
}

.project_container {
    margin: 40px auto;
    width: 90%;
}

.little_header img {
    width: 100% !important;
}

.little_header {
    display: flex;
    flex-direction: row;
    justify-content: start;
    align-items: center;
    gap: 30px;
    color: #1C1B1B;
    font-size: 105px;
    line-height: 60px;
    font-family: ReportFont;
    font-weight: 400;
    text-align: left;
    width: 100%;
}

.img_row {
    display: flex;
    gap: 30px;
    margin-top: 30px;
    justify-content: center;
    align-items: center;
}



.artist_year {
    font-family: BrinnanThin !important;
    font-size: 16px;
    font-weight: 400;
    line-height: 13px;
    letter-spacing: 0em;
    text-align: justified;
    color: #ffffff;

}

.artist_name {
    font-family: BrinnanBold !important;
    font-size: 30px;
    font-weight: 900;
    line-height: 40px;
    letter-spacing: 0em;
    text-align: justified;
    color: #ffffff;

}

/*  */
.container {
    width: auto;
    position: relative;
    overflow: hidden;
}

.container img {
    width: 100%;
    height: auto;
}

.container:hover .t {
    top: -4px;
}

.t img {
    width: 50px;
    height: 50px;
}

.t {
    color: white;
    background: #FF540B99;
    position: absolute;
    top: -100%;
    height: 100%;
    width: 100%;
    padding: 10px;
    /* border-radius: 35px; */
    box-sizing: border-box;
    transition: all 0.4s;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: end;
    gap: 40px;
}

.mobile_friendly {
    display: none;
}

.main_img img {
    width: 100%;
    border-radius: 30px !important;

}

/*  */

@media only screen and (max-width: 1100px) {
    .mobile_friendly {
        display: block;
    }

    .project_container {
        margin: 40px auto;
        width: 100%;

    }

    .img_row:nth-child(even) {
        flex-direction: column-reverse;

    }

    .main_img img {
        width: 100%;
    }

    .img_row {
        flex-direction: column;
    }

    .project_images {
        margin: 30px !important;
        display: none;
    }

    .little_header {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 0;
        color: #1C1B1B;
        font-family: ReportFont;
        font-weight: 400;
        width: 100%;
        font-size: 50px;
        line-height: 70px;
        text-align: center;
    }

    .little_header img {
        display: none;
    }


}
</style>