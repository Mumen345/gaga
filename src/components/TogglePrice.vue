<template>
    <div>
        <div v-if="isActive2" class="">
            <div class="wrapper">
                <div class="pricing-table gprice-single">
                    <div class="head">
                        <h4 class="title">Basic</h4>
                    </div>
                    <div class="content">
                        <div class="price">
                            <h1>$19</h1>
                        </div>
                        <ul>
                            <li>5 GB Ram</li>
                            <li>40GB SSD Cloud Storage</li>
                            <li>Month Subscription</li>
                            <li>Responsive Framework</li>
                            <li> <del>Monthly Billing Software</del> </li>
                            <li> <del>1 Free Website</del></li>

                        </ul>
                        <div class="sign-up">
                            <a href="#" class="btn bordered radius">Signup Now</a>
                        </div>
                    </div>
                </div>
                <div class="pricing-table gprice-single">
                    <div class="head">
                        <h4 class="title">Standard</h4>
                    </div>
                    <div class="content">
                        <div class="price">
                            <h1>$29</h1>
                        </div>
                        <ul>
                            <li>5 GB Ram</li>
                            <li>40GB SSD Cloud Storage</li>
                            <li>Month Subscription</li>
                            <li>Responsive Framework</li>
                            <li>Monthly Billing Software</li>
                            <li><del>1 Free Website</del></li>

                        </ul>
                        <div class="sign-up">
                            <a href="#" class="btn bordered radius">Signup Now</a>
                        </div>
                    </div>
                </div>
                <div class="pricing-table gprice-single">
                    <div class="head">
                        <h4 class="title">Premium</h4>
                    </div>
                    <div class="content">
                        <div class="price">
                            <h1>$39</h1>
                        </div>
                        <ul>
                            <li>5 GB Ram</li>
                            <li>40GB SSD Cloud Storage</li>
                            <li>Month Subscription</li>
                            <li>Responsive Framework</li>
                            <li>Monthly Billing Software</li>
                            <li>1 Free Website</li>
                        </ul>
                        <div class="sign-up">
                            <a href="#" class="btn bordered radius">Signup Now</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div v-if="isActive">
            <div class="wrapper">
                <div class="pricing-table gprice-single">
                    <div class="head">
                        <h4 class="title">Basic</h4>
                    </div>
                    <div class="content">
                        <div class="price">
                            <h1>$19</h1>
                        </div>
                        <ul>
                            <li>5 GB Ram</li>
                            <li>40GB SSD Cloud Storage</li>
                            <li>Month Subscription</li>
                            <li>Responsive Framework</li>
                            <li> <del>Monthly Billing Software</del> </li>
                            <li> <del>1 Free Website</del></li>

                        </ul>
                        <div class="sign-up">
                            <a href="#" class="btn bordered radius">Signup Now</a>
                        </div>
                    </div>
                </div>
                <div class="pricing-table gprice-single">
                    <div class="head">
                        <h4 class="title">Standard</h4>
                    </div>
                    <div class="content">
                        <div class="price">
                            <h1>$29</h1>
                        </div>
                        <ul>
                            <li>5 GB Ram</li>
                            <li>40GB SSD Cloud Storage</li>
                            <li>Month Subscription</li>
                            <li>Responsive Framework</li>
                            <li>Monthly Billing Software</li>
                            <li><del>1 Free Website</del></li>

                        </ul>
                        <div class="sign-up">
                            <a href="#" class="btn bordered radius">Signup Now</a>
                        </div>
                    </div>
                </div>
                <div class="pricing-table gprice-single">
                    <div class="head">
                        <h4 class="title">Premium</h4>
                    </div>
                    <div class="content">
                        <div class="price">
                            <h1>$39</h1>
                        </div>
                        <ul>
                            <li>5 GB Ram</li>
                            <li>40GB SSD Cloud Storage</li>
                            <li>Month Subscription</li>
                            <li>Responsive Framework</li>
                            <li>Monthly Billing Software</li>
                            <li>1 Free Website</li>
                        </ul>
                        <div class="sign-up">
                            <a href="#" class="btn bordered radius">Signup Now</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "TogglePrice",
    data() {
        return {
            isActive: true,
            isActive2: false,
        };
    },
    methods: {
        showmonthly: function () {
            this.isActive = true;
            this.isActive2 = false;
        },
        showAnually: function () {
            this.isActive2 = true;
            this.isActive = false;
        }
    },
}
</script>

<style lang="scss" scoped></style>