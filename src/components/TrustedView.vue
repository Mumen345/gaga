<template>
    <div>
        <p class="little_header">Our Service <span><img src="../assets/images/long_arrow.svg" alt="arrow"></span> </p>

        <div class="trusted_container">
            <div class="sliding_background"></div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.trusted_container {
    overflow: hidden;
}

.sliding_background {
    background: url("../assets/images/trusted_img.png") repeat-y;
    width: 100%;
    --imageHeight: 400px;
    height: calc(var(--imageHeight) * 2);
    animation: slide 4s linear infinite;
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
    font-family: BrinnanRegular;
    color: #1C1B1B;
    font-size: 32px;
    font-weight: 400;
    line-height: 38px;
    letter-spacing: 0em;
    text-align: left;
    width: 100%;

}


@keyframes slide {
    from {
        transform: translateY(0px);
    }

    to {
        transform: translateY(calc(var(--imageHeight) * -1));
    }
}

@media only screen and (max-width: 1034px) {
    .little_header {
        display: none;

    }

}
</style>