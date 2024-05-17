<template>
    <div class="pp_container">
        <div class="toggle_toggle">
            <div class="text_container" @click="showmonthly" :class="{ active: isActive }">
                <p>Monthly</p>

            </div>
            <div class="text_container" @click="showAnually" :class="{ active: isActive2 }">
                <p>Annual <span>
                        Save 30%
                    </span> </p>
            </div>
        </div>
        <div v-if="isActive2" class="">
            <div id="container" class="body">
                <div class="whole">
                    <div class="type">
                        <p>Simple</p>
                    </div>
                    <div class="plan">

                        <div class="header">
                            <span>$</span>1.5K<sup></sup>
                            <p class="month">Yearly</p>
                        </div>
                        <div class="content">
                            <ul>
                                <li>Brand Strategy</li>
                                <li>Brand Identity </li>
                                <li>Branding</li>
                                <li>Content Strategy</li>
                                <li>Content Consultancy</li>
                                <li>Content Calendar</li>
                                <li>TikTok Videos</li>
                                <li>Instagram Reels</li>
                                <li class="color_change">
                                    <del>

                                        Promo Videos
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Lifestyle Videos
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Studio Shots
                                    </del>
                                </li>
                                <li>Lifestyle Shots</li>
                                <li>Marketing graphics </li>
                                <li class="color_change">
                                    <del>
                                        3d Graphics
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Motion Graphics
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Illustrations
                                    </del>
                                </li>
                                <li>Meta(Facebook, Instagram)</li>
                                <li class="color_change">
                                    <del>
                                        Twitter (X)
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        YouTube
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Snapchats
                                    </del>
                                </li>
                                <li>Influencers (Micro)</li>
                                <li>Influencers (Macro)</li>
                                <li>Website</li>
                            </ul>

                        </div>
                    </div>
                </div>
                <div class="whole">
                    <div class="type standard">
                        <p>Standard</p>
                    </div>
                    <div class="plan">

                        <div class="header">
                            <span>$</span>2K<sup></sup>
                            <p class="month">Yearly</p>
                        </div>
                        <div class="content">
                            <ul>
                                <li>Brand Strategy</li>
                                <li>Brand Identity </li>
                                <li>Branding</li>
                                <li>Content Strategy</li>
                                <li>Content Consultancy</li>
                                <li>Content Calendar</li>
                                <li>TikTok Videos</li>
                                <li>Instagram Reels</li>
                                <li class="color_change">
                                    <del>
                                        Promo Videos
                                    </del>
                                </li>
                                <li>Lifestyle Videos</li>
                                <li>Studio Shots</li>
                                <li>Lifestyle Shots</li>
                                <li>Marketing graphics </li>
                                <li>3d Graphics</li>
                                <li class="color_change">
                                    <del>
                                        Motion Graphics
                                    </del>
                                </li>
                                <li>Illustrations</li>
                                <li>Meta(Facebook, Instagram)</li>
                                <li>Twitter (X)</li>
                                <li>YouTube</li>
                                <li class="color_change">
                                    <del>
                                        Snapchats
                                    </del>
                                </li>
                                <li>Influencers (Micro)</li>
                                <li>Influencers (Macro)</li>
                                <li>Website</li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div class="whole ">
                    <div class="type ultimate">
                        <p>Ultimate</p>
                    </div>
                    <div class="plan">

                        <div class="header">
                            <span>$</span>3K<sup></sup>
                            <p class="month">Yearly</p>
                        </div>
                        <div class="content">
                            <ul>
                                <li>Brand Strategy</li>
                                <li>Brand Identity </li>
                                <li>Branding</li>
                                <li>Content Strategy</li>
                                <li>Content Consultancy</li>
                                <li>Content Calendar</li>
                                <li>TikTok Videos</li>
                                <li>Instagram Reels</li>
                                <li>Promo Videos</li>
                                <li>Lifestyle Videos</li>
                                <li>Studio Shots</li>
                                <li>Lifestyle Shots</li>
                                <li>Marketing graphics </li>
                                <li>3d Graphics</li>
                                <li>Motion Graphics</li>
                                <li>Illustrations</li>
                                <li>Meta(Facebook, Instagram)</li>
                                <li>Twitter (X)</li>
                                <li>YouTube</li>
                                <li>Influencers</li>
                                <li>Micro</li>
                                <li>Macro</li>
                                <li>Website</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div v-if="isActive">
            <div id="container" class="body">
                <div class="whole">
                    <div class="type">
                        <p>Simple</p>
                    </div>
                    <div class="plan">

                        <div class="header">
                            <span>$</span>137<sup></sup>
                            <p class="month">Monthly</p>
                        </div>
                        <div class="content">
                            <ul>
                                <li>Brand Strategy</li>
                                <li>Brand Identity </li>
                                <li>Branding</li>
                                <li>Content Strategy</li>
                                <li>Content Consultancy</li>
                                <li>Content Calendar</li>
                                <li>TikTok Videos</li>
                                <li>Instagram Reels</li>
                                <li class="color_change">
                                    <del>

                                        Promo Videos
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Lifestyle Videos
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Studio Shots
                                    </del>
                                </li>
                                <li>Lifestyle Shots</li>
                                <li>Marketing graphics </li>
                                <li class="color_change">
                                    <del>
                                        3d Graphics
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Motion Graphics
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Illustrations
                                    </del>
                                </li>
                                <li>Meta(Facebook, Instagram)</li>
                                <li class="color_change">
                                    <del>
                                        Twitter (X)
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        YouTube
                                    </del>
                                </li>
                                <li class="color_change">
                                    <del>
                                        Snapchats
                                    </del>
                                </li>
                                <li>Influencers (Micro)</li>
                                <li>Influencers (Macro)</li>
                                <li>Website</li>
                            </ul>

                        </div>

                    </div>
                </div>
                <div class="whole">
                    <div class="type standard">
                        <p>Standard</p>
                    </div>
                    <div class="plan">

                        <div class="header">
                            <span>$</span>182<sup></sup>
                            <p class="month">Monthly</p>
                        </div>
                        <div class="content">
                            <ul>
                                <li>Brand Strategy</li>
                                <li>Brand Identity </li>
                                <li>Branding</li>
                                <li>Content Strategy</li>
                                <li>Content Consultancy</li>
                                <li>Content Calendar</li>
                                <li>TikTok Videos</li>
                                <li>Instagram Reels</li>
                                <li class="color_change">
                                    <del>
                                        Promo Videos
                                    </del>
                                </li>
                                <li>Lifestyle Videos</li>
                                <li>Studio Shots</li>
                                <li>Lifestyle Shots</li>
                                <li>Marketing graphics </li>
                                <li>3d Graphics</li>
                                <li class="color_change">
                                    <del>
                                        Motion Graphics
                                    </del>
                                </li>
                                <li>Illustrations</li>
                                <li>Meta(Facebook, Instagram)</li>
                                <li>Twitter (X)</li>
                                <li>YouTube</li>
                                <li class="color_change">
                                    <del>
                                        Snapchats
                                    </del>
                                </li>
                                <li>Influencers (Micro)</li>
                                <li>Influencers (Macro)</li>
                                <li>Website</li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div class="whole ">
                    <div class="type ultimate">
                        <p>Ultimate</p>
                    </div>
                    <div class="plan">

                        <div class="header">
                            <span>$</span>273<sup></sup>
                            <p class="month">Monthly</p>
                        </div>
                        <div class="content">
                            <ul>
                                <li>Brand Strategy</li>
                                <li>Brand Identity </li>
                                <li>Branding</li>
                                <li>Content Strategy</li>
                                <li>Content Consultancy</li>
                                <li>Content Calendar</li>
                                <li>TikTok Videos</li>
                                <li>Instagram Reels</li>
                                <li>Promo Videos</li>
                                <li>Lifestyle Videos</li>
                                <li>Studio Shots</li>
                                <li>Lifestyle Shots</li>
                                <li>Marketing graphics </li>
                                <li>3d Graphics</li>
                                <li>Motion Graphics</li>
                                <li>Illustrations</li>
                                <li>Meta(Facebook, Instagram)</li>
                                <li>Twitter (X)</li>
                                <li>YouTube</li>
                                <li>Influencers</li>
                                <li>Micro</li>
                                <li>Macro</li>
                                <li>Website</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Our Services",
    data() {
        return {
            isActive: true,
            isActive2: false,
        }
    },
    methods: {
        showmonthly: function () {
            this.isActive = true;
            this.isActive2 = false
        },
        showAnually: function () {
            this.isActive2 = true
            this.isActive = false;
        }

    }
}
</script>

<style scoped>
.color_change {
    color: #eac80d;
}

.pp_container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 30px;
    width: 100%;
    margin: 0 auto;
    background-color: #f5f8fa;
    padding-top: 60px;
    padding-bottom: 60px;
}

.toggle_toggle {
    background: #EEEEEE;
    height: 75px;
    left: 455px;
    border-radius: 150px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 30px;
    padding: 10px;
    font-family: BrinnanBold;
}

.active {
    background: #171717;
    color: #ffffff;

}

.text_container {
    width: 203px;
    height: 70px;
    padding: 36px, 49px;
    border-radius: 88.39px;
    gap: 10px;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;

}






input:focus,
textarea:focus,
select:focus {
    border: 1px solid #fafafa;
    -webkit-box-shadow: 0 0 6px #007eff;
    -moz-box-shadow: 0 0 5px #007eff;
    box-shadow: 0 0 5px #007eff;
    outline: none;
}

sup {

    font-size: 40px;
}

ul {
    list-style: none;
    font-size: 15px;
    font-family: BrinnanRegular;
    color: #9095aa;
    padding: 0px;
    margin: 0px;


}


li {
    border-bottom: 1px solid #494a5a;
    padding: 0px;
    margin: 0px;
    text-align: center;
    height: 52px;
    line-height: 52px;
}


#container {
    width: 100%;
    text-align: center;
    display: flex;
    flex-direction: row;
    gap: 30px;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.whole {
    display: inline-block;

}



.type {
    width: 300px;
    border-radius: 5px 5px 0px 0px;
    background-color: #eac80d;
    height: 62px;
    border-bottom: 3px solid #bfa30c;

}

.type p {
    font-family: BrinnanRegular;
    font-weight: 800;
    font-size: 29px;
    text-transform: uppercase;
    color: white;
    text-align: center;
    padding-top: 10px;



}

.plan {
    width: 300px;
    background-color: #2b2937;

    border-radius: 0px 0px 5px 5px;
    font-family: BrinnanRegular;
    font-size: 90px;
    color: white;
    text-align: center;


}

.standard {
    background-color: #1abc9c;
    border-bottom: 3px solid #18937b;
}

.ultimate {
    background-color: #5d6a9a;
    border-bottom: 3px solid #474f6f;
}





.header {
    border-bottom: 1px solid #494a5a;
    padding-bottom: 39px;


}

.header span {
    font-size: 32px;


}

.month {
    font-size: 14px;
    color: #575757;
    padding: 0px;
    margin: -10px;
}

.price {
    height: 80px;
}

.cart {

    color: white;
    position: relative;
    top: 16px;

}

.bottom {}

.content {}

.login_c {
    width: 500px;
    background-color: #2b2937;
    height: 300px;
    margin: 0 auto;
    margin-top: 40px;
    border-radius: 5px;

}

.login_c input {
    width: 350px;
    height: 40px;
    border: 1px solid #494a5a;
    margin-bottom: 20px;
    border-radius: 5px;
    padding-left: 10px;

}


.login {
    background-color: #BC4B1A;
    border-bottom: 3px solid #7C3618;
    width: 100%;

}

.top {
    margin-top: 35px;
}

.nodisplay {
    opacity: 0.1;
}

.selected {
    background-color: #1F1B36;
    margin: 0px;
    padding: 0px;
}

@media only screen and (max-width: 1291px) {
    .price_container {
        display: flex;
        flex-direction: row;
        gap: 30px;
        justify-content: center;
        color: #ffffff;
        flex-wrap: wrap;
        width: 90%;
        margin: 0 auto;
    }
}

@media only screen and (max-width: 704px) {
    .toggle_toggle {
        background: #EEEEEE;
        height: 82px;
        border-radius: 150px;
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 30px;
        padding: 10px;
        font-family: BrinnanBold;
        width: 90%;
        margin: 0 auto;
        box-sizing: border-box;
    }
}
</style>