<template>
<div class="container">
    <nav class="navbar">
        <p>LOGO</p>

        <div class="links">
            <router-link to="#">About us</router-link>
            <router-link to="#">Services</router-link>

        </div>
        <button @click="goTocontact" class="secondarybtn"> Let's Talk</button>
    </nav>
    <div class="topnav">
        <a href="#home" class="active">Logo</a>
        <div id="myLinks">
            <router-link to="/about">About us</router-link>
            <router-link to="/services">Services</router-link>
            <router-link to="/pricing">Pricing</router-link>
            <router-link to="/contact">Let's Talk</router-link>

        </div>
        <a href="javascript:void(0);" class="icon" @click="myFunctiion">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3.75 6.75H20.25M3.75 12H12M3.75 17.25H20.25" stroke="black" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
            </svg>

        </a>
    </div>
</div>
</template>

<script>
export default {
    name: "NavigationBar",
    methods: {
        goTocontact() {
            this.$router.push("/contact")
        },
        myFunctiion() {
            var x = document.getElementById("myLinks");
            if (x.style.display === "block") {
                x.style.display = "none";
            } else {
                x.style.display = "block";
            }

        }
    }
}
</script>

<style scoped>
.container {
    display: flex;
    background-color: #a8a8a800;
    width: 100% !important;
    justify-content: space-around;
    height: 103px;
    border-bottom: 1px solid #C2C2C2;
    z-index: 0;
}

.navbar {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 100%;
}

.links {
    display: flex;
    gap: 20px;
}

a {
    color: #ffffff;
    text-decoration: none;
    font-family: BrinnanRegular;
}

/* Responsive Menu */
.topnav {
    display: none;

}

@media only screen and (max-width: 1000px) {

    .navbar {
        display: none;
    }

    .topnav {
        overflow: hidden;
        background-color: #ffffff00;
        position: relative;
        display: block;
        width: 100%;
        transition: height 4s;

    }

    .topnav #myLinks {
        display: none;
    }

    .topnav a {
        color: #2A2929;
        padding: 14px 16px;
        text-decoration: none;
        font-size: 15px;
        display: block;
    }

    .topnav a.icon {
        background: #b3a2a200;
        display: block;
        position: absolute;
        right: 0;
        top: 0;
    }

    .topnav a:hover {
        background-color: #ffffff00;
        color: black;
    }

    .active {
        background-color: #ffffff;
        color: rgb(0, 0, 0);
    }

    .container {
        display: flex;
        background-color: #ffffff;
        width: 100%;
        justify-content: end;
        height: auto;
        border-bottom: 1px solid #C2C2C2;
        z-index: 0;
        transition: height 4s;
    }
}
</style>
