<template>
    <div class="header_div">
        <p class="plans_header">FLEXIBLE PRICING PLANS FOR YOUR BRAND</p>
        <p class="subtext">Lorem ipsum dolor sit amet consectetur. Lacus rutrum feugiat adipiscing parturient non </p>
        <PricePlan />
    </div>
</template>

<script>
import PricePlan from './PricePlan.vue';

export default {
    components: { PricePlan }
}
</script>

<style scoped>
.plans_header {
    font-family: ReportSchoolW00-Heavy;
    font-size: 90px;
    font-weight: 900;
    line-height: 116px;
    letter-spacing: 0em;
    text-align: left;
    text-transform: capitalize !important;
    text-align: center;
    width: 100%;
}

.subtext {
    font-family: BrinnanLight;
    font-size: 18px;
    font-weight: 400;
    line-height: 21px;
    letter-spacing: 0em;
    text-align: justified;
    text-align: center;
    width: 100%;
}



.header_div {
    display: flex;
    flex-direction: column;
    gap: 30px;
    justify-content: center;
    align-items: center;
}

.header_div img {
    width: 100%;
}

@media only screen and (max-width: 1034px) {
    .header_div img {
        display: none;
    }

    .plans_header {
        font-size: 50px;
        line-height: 70px;
        text-align: center;
    }
}
</style>