<template>
    <div class="service_section">
        <div class="left_div">
            <p class="little_header">Our Service <span><img src="../assets/images/long_arrow.svg" alt="arrow"></span> </p>
            <div class="writeup_div">
                <p class="header">OUR <span class="bold_text">
                        SERVICES
                    </span> </p>
                <p v-if="isActive" class="writeup">We produce high quality content tailored to the creative needs, goals and
                    target
                    audience. This could
                    involve
                    filming, designing, and recording contents. <br>
                    We have high level production equipment at our disposal to match any content needed.</p>
                <p v-if="isActive2" class="writeup">
                    We brainstorm and devise a plan outlining what type of content will be created to best fit the creative
                    which would also help in the branding/rebranding. We outline the content, where it would be published,
                    and how it would align with the creative goals.
                </p>
                <p v-if="isActive3" class="writeup">
                    We assist in distributing and promoting the content across all platforms to increase visibility and
                    reach the intended audience.
                </p>
                <p v-if="isActive4" class="writeup">
                    We offer insights into content performance through analytics tools, allowing creatives to track the
                    success of their content campaigns.
                </p>

            </div>
        </div>
        <div class="right_div">
            <div @click="toggleActive" :class="{ active: isActive }">
                <p>Content Creation</p>

            </div>
            <div @click="toggleTwo" :class="{ active: isActive2 }">
                <p>Content Strategy</p>

            </div>
            <div @click="toggleThree" :class="{ active: isActive3 }">

                <p>Content Marketing</p>
            </div>
            <div @click="toggleFour" :class="{ active: isActive4 }">
                <p>Analytics and Reporting</p>

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
            isActive3: false,
            isActive4: false,
        }
    },
    methods: {
        toggleActive: function () {
            this.isActive = true;
            this.isActive2 = false
            this.isActive3 = false
            this.isActive4 = false
        },
        toggleTwo: function () {
            this.isActive2 = true;
            this.isActive = false;
            this.isActive3 = false;
            this.isActive4 = false;
        },
        toggleThree: function () {
            this.isActive3 = true
            this.isActive2 = false
            this.isActive4 = false
            this.isActive = false;
        },
        toggleFour: function () {
            this.isActive4 = true
            this.isActive3 = false
            this.isActive2 = false
            this.isActive = false;
        }
    }
}
</script>

<style  scoped>
.little_header img {
    width: 100% !important;
}

.header {
    font-size: 128px;
    line-height: 151.81px;
    font-family: ReportFont;
    font-weight: 400;
}

.bold_text {}

.writeup_div {
    width: 554px;
    height: 497px;
    top: 86px;
    gap: 12px;
    display: flex;
    flex-direction: column;
    gap: 30px;
    justify-content: center;
    align-items: center;

}

.writeup {
    font-family: BrinnanLight !important;
    font-size: 20px !important;
    font-weight: 300;
    line-height: 24px;
    letter-spacing: 0em;
    text-align: justify;
    width: 390px;
    height: 177px;
    color: #474747;

}

.little_header {
    display: flex;
    flex-direction: row;
    justify-content: start;
    align-items: center;
    gap: 30px;
    font-family: BrinnanRegular;
    color: #1C1B1B;
    font-size: 32px;
    font-weight: 400;
    line-height: 38px;
    letter-spacing: 0em;
    text-align: left;
    width: 100%;

}



.left_div {
    display: flex;
    flex-direction: column;
    width: 554px;
}

.service_section {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    justify-content: space-between;
    background-color: #F6F6F6;
    padding: 69px;
    align-items: center;
}

.right_div div {
    font-family: BrinnanBold;
    font-size: 32px;
    font-weight: 900;
    letter-spacing: 0em;
    text-align: left;
    color: #909090;
    border-bottom: 1px solid #CFCFCF;
    height: 120px;
    background-color: #F6F6F6;
    display: flex;
    justify-content: start;
    align-items: center;
    padding-left: 30px;
    cursor: pointer;

}

.right_div {
    display: flex;
    text-align: left;
    flex-direction: column;
    width: 45%;
}

.active {
    background-color: #D9D9D9 !important;
    color: #1B1A1A !important;
}

@media only screen and (max-width: 1295px) {
    .left_div {
        display: flex;
        flex-direction: column;
        width: 454px;
    }

    .header {
        font-size: 100px;
        line-height: 120px;
        font-family: ReportFont;
        font-weight: 400;
    }

    .writeup {
        /* font-family: BrinnanBold; */
        font-size: 20px !important;
        font-weight: 300;
        line-height: 24px;
        letter-spacing: 0em;
        text-align: justify;
        width: 390px;
        height: auto;


    }

    .writeup_div {
        width: auto;
        height: 497px;
        display: flex;
        flex-direction: column;
        gap: 30px;
        justify-content: start;
        align-items: start;

    }

    @media only screen and (max-width: 1034px) {

        .left_div {
            display: flex;
            flex-direction: column;
            width: 100%;
            justify-content: center;
            align-items: center;
        }

        .writeup_div {
            width: auto;
            height: 100%;
            display: flex;
            flex-direction: column;
            gap: 10px;
            justify-content: start;
            align-items: center;

        }

        .writeup {
            width: 100%;
            text-align: center;
            line-height: 35px;
        }

        .little_header {
            display: none;

        }

        .right_div {
            display: flex;
            text-align: left;
            flex-direction: column;
            width: 100%;
        }

        .service_section {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: space-between;
            background-color: #F6F6F6;
            padding: 20px;
            align-items: center;
        }

        .header {
            font-size: 50px;
            line-height: 60px;
            font-family: ReportFont;
            font-weight: 400;
        }
    }
}
</style>