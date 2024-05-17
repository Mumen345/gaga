<template>
    <div class="counter_div">
        <div>
            <p class="counter">

                <countTo :startVal='0' :endVal='200' :duration='3000' :suffix='surfix' :autoplay=true></countTo>+
            </p>
            <p class="bottom_text">Talent managed</p>
        </div>
        <div>
            <p class="counter">

                <countTo :startVal='0' :endVal='100' :duration='3000' :suffix='surfix' :autoplay=true></countTo>+
            </p>
            <p class="bottom_text">Talent managed</p>
        </div>


    </div>
</template>
   
<script>
import countTo from 'vue-count-to';
export default {
    components: { countTo },
    data() {
        return {
            startVal: 0,
            endVal: 2017,
            separator: ",",
            suffix: "+",


        }
    }
}
</script>
<style scoped>
.counter {
    font-family: BrinnanBold !important;
    font-size: 40px;
    font-weight: 900;
    line-height: 48px;
    letter-spacing: 0em;
    text-align: left;
    font-weight: 900;
    color: #ffffff;
}

.counter_div {
    display: flex;
    gap: 30px;
    padding: 10px 30px;
    width: 300px;

}

.bottom_text {
    color: #ffffff;
    font-family: Brinnan;
    font-size: 16px;
    font-weight: 400;
    line-height: 19px;
    letter-spacing: 0em;
    text-align: left;

}
</style>