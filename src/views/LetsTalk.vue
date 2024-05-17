<template>
    <div>
        <NavigationBar />
        <div class="contact_container">
            <div class="contact_firstDiv">
                <div class="text_img">
                    <p>LET'S</p> <img src="../assets/images/four_rings.svg" alt=""> <br />
                </div>
                <div class="text_img">
                    <img src="../assets/images/small_star.svg" alt="">
                    <p>GET </p>
                    <p>IN</p> <br />
                </div>
                <p>TOUCH</p>
            </div>
            <p class="mobile_view">GET IN TOUCH</p>
            <div class="form_container">
                <Label for="name">Full Name</Label>
                <input id="name" type="text" v-model="request.fullName">
                <Label id="brandname" for="brand">Brand</Label>
                <input type="text" v-model="request.brandName">
                <Label for="brand">Email</Label>
                <input id="email" type="email" v-model="request.email">
                <button class="send_button" @click.prevent="submitForm">Send
                    <img src="../assets/images/arrow_varient.svg" alt="">
                </button>
            </div>
        </div>
        <FooterView />
        <BaseFooter />
    </div>
</template>
  
<script>
import BaseFooter from '@/components/BaseFooter.vue';
import FooterView from '@/components/FooterView.vue';
import NavigationBar from '@/components/NavigationBar.vue';
import axios from "axios";

export default {
    name: "LetsTalk",
    data() {
        return {
            request: {
                fullName: "",
                brandName: "",
                email: "",

            }
        }
    },
    methods: {
        validateEmail(email) {
            const re =
                /^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))*$/;
            return re.test(email);
        },
        submitForm() {
            if (this.request.fullName === "") {
                this.$toasted.error("Please tell us your name", {
                    position: "top-right",
                    duration: 5000
                });
                return false;
            }
            if (this.request.brandName === "") {
                this.$toasted.error("Please tell us your brand", {
                    position: "top-right",
                    duration: 5000
                });
                return false;
            }
            if (this.request.email === "") {
                this.$toasted.error("Please fill your email", {
                    position: "top-right",
                    duration: 5000
                });
                return false;
            }
            if (this.request.email === "") {
                this.$toasted.error("Please fill your email", {
                    position: "top-right",
                    duration: 5000
                });
                return false;
            }
            if (!this.validateEmail(this.request.email)) {
                this.$toasted.error("Invalid email address", {
                    position: "top-right",
                    duration: 5000
                });
                return false;
            }
            // const params = "email=" + this.request;
            // console.log(params);
            axios
                // .post("https://jsonplaceholder.typicode.com/" + params)
                .post("https://jsonplaceholder.typicode.com/", this.request)

                .then((response) => {
                    // console.log(response.status);
                    if (response.status === 200 && response.data.status === "ok") {
                        this.$toasted.success("Success! Thank you for your Response", {
                            position: "top-right",
                            duration: 5000
                        });
                        this.email = "";
                    } else {
                        this.$toasted.error("oops an error occurred", {
                            position: "top-right",
                            duration: 5000
                        });
                        return false;
                    }
                })
                .catch((error) => {
                    console.log(error);
                    this.$toasted.error("Try rest, we don't have a backend yet", {
                        position: "top-right",
                        duration: 5000
                    });
                });
        },
        showInput() {
            this.inputDiv = true;
            this.mainButton = false;
        },
    },
    components: { NavigationBar, FooterView, BaseFooter }
}
</script>
  
<style scoped>
.mobile_view {
    display: none;
}

.contact_container {
    display: flex;
    gap: 30px;
    width: 80%;
    margin: 50px auto;
    justify-content: space-between;
    align-items: center;
}

.contact_firstDiv img {
    /* width: 100%; */
}

.contact_firstDiv {
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-items: start;
    width: 100%;
}

.text_img {
    display: flex;
    align-items: center;
    width: 500px;
    gap: 14px;
    justify-content: center;
}

p {
    font-family: ReportFont;
    font-size: 120px;
    font-weight: 900;
    line-height: 153.6px;
    letter-spacing: 0em;
    text-align: center;
    color: #2A2929;


}

label {
    font-family: BrinnanRegular;
    font-size: 24px;
    font-weight: 400;
    line-height: 29px;
    letter-spacing: 0em;
    text-align: left;
    color: #696969;

}

input[type=email] {
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    border: none;
    box-sizing: border-box;
    outline: none;
    font-size: 14px;
    font-family: BrinnanRegular;
    border-bottom: 1px solid #CFCFCF;
    color: #696969;
}

input[type=text] {
    border: none;
    width: 100%;
    padding: 12px 20px;
    margin: 8px 0;
    box-sizing: border-box;
    outline: none;
    font-family: BrinnanRegular;
    font-size: 14px;
    border-bottom: 1px solid #CFCFCF;
    color: #696969;
}

.form_container {
    display: flex;
    flex-direction: column;
    justify-content: start;
    align-items: start;
    gap: 10px;
    box-sizing: border-box;
    width: 70%;
}

.send_button {
    width: 150px;
    padding: 20px;
    border-radius: 34px;
    border: 1px solid #2A2929;
    gap: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #ffffff;
    height: 64px;
    font-family: BrinnanRegular;
    font-weight: 400;
    line-height: 21px;
    letter-spacing: 0em;
    font-size: 18px;
}

@media only screen and (max-width: 1100px) {
    .contact_container {
        width: 95%;
        margin: 50px auto;
        justify-content: space-between;
        align-items: center;
        gap: 0px;
    }
}

@media only screen and (max-width: 1000px) {
    .contact_container {
        width: 95%;
        margin: 50px auto;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 0px;
    }

    .contact_firstDiv {
        justify-content: center;
        align-items: center;
    }

    .contact_firstDiv img {
        display: none;
    }

    .mobile_view {
        display: block;
        margin-bottom: 50px !important;
        font-size: 70px;
        line-height: normal;
        color: #2A2929;
    }

    .contact_firstDiv {
        display: none;
    }

    .form_container {
        width: 100%;
        gap: 0;

    }

    input[type=email] {
        width: 100%;
        padding: 12px 20px;
        margin: 8px 0;
        border: none;
        border-bottom: 1px solid #CFCFCF;
        box-sizing: border-box;
        outline: none;
    }

    input[type=text] {
        border: none;
        width: 100%;
        padding: 12px 20px;
        margin: 8px 0;
        border-bottom: 1px solid #CFCFCF;
        box-sizing: border-box;
        outline: none;
    }

    .send_button {
        width: 100%;
        margin-top: 40px;
    }
}
</style>