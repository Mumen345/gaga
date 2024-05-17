<template>
    <div class="sm_footer_container">
        <img src="../assets/images/LOGO.svg" alt="">
        <div class="bottom_footer">
            <p>
                <router-link to="/pricing">TERMS & AGREEMENTS</router-link>
            </p>
            <p>
                <router-link to="/pricing">@2023BRANDNAME ALL RIGHT RESERVED</router-link>
            </p>
            <p>
                <router-link to="/pricing">PRIVACY & POLICY</router-link>
            </p>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.sm_footer_container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 30px;
    margin-top: 50px;
    margin-bottom: 70px;
}

a {
    font-family: BrinnanRegular;
    font-size: 24px;
    font-weight: 400;
    line-height: 29px;
    letter-spacing: 0em;
    text-align: center;
    cursor: pointer;
}

.bottom_footer {
    display: flex;
    gap: 30px;
    text-align: center;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}
</style>