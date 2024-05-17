<template>
    <div class="second_section">
        <marquee direction="left" behavior="">
            <p>LET'S CREATE BEST BRAND WITH OUR EXPERIENCE</p>
        </marquee>
        <div>
            <CounterView />
        </div>
    </div>
</template>

<script>
import CounterView from './CounterView.vue';

export default {
    components: { CounterView }
}
</script>

<style scoped>
.second_section {
    margin-top: 40px;
    background: #2A2929;
    height: auto;
    padding: 10px 0;
    display: flex;
    /* flex-wrap: wrap; */
    justify-content: center;
    align-items: center;
    width: 100%;

}

.second_section p {
    font-family: Brinnan;
    font-size: 48px;
    font-weight: 400;
    line-height: 57px;
    letter-spacing: 0em;
    text-align: left;
    width: 70%;
    color: #ffffff;

}

@media only screen and (max-width: 700px) {
    .second_section {
        flex-wrap: wrap;
        padding-bottom: 30px;
    }

}
</style>