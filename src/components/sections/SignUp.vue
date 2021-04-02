<template>
    <section class="signup-section" id="signup">
        <div class="container">
            <div class="row">
                <div class="col-md-10 col-lg-8 mx-auto text-center">
                    <i class="far fa-paper-plane fa-2x mb-2 text-white"></i>
                    <h2 class="text-white mb-5">
                        Subscribe to receive updates!
                    </h2>
                    <form class="form-inline d-flex">
                        <input
                            class="form-control flex-fill mr-0 mr-sm-2 mb-3 mb-sm-0"
                            id="inputEmail"
                            type="email"
                            placeholder="Enter email address..."
                        />
                        <button class="btn btn-primary mx-auto" type="submit">
                            Subscribe
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "SignUp",
});
</script>

<style lang="scss" scoped>
@import "~@/assets/scss/styles.scss";

.signup-section {
    padding: 10rem 0;
    background: linear-gradient(
            to bottom,
            #{fade-out($black, 0.9)} 0%,
            #{fade-out($black, 0.5)} 75%,
            $black 100%
        ),
        url("~@/assets/img/bg-signup.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: scroll;
    background-size: cover;
    .form-inline {
        input {
            box-shadow: 0 0.1875rem 0.1875rem 0 rgba(0, 0, 0, 0.1) !important;
            padding: 1.25rem 2rem;
            height: auto;
            font-family: $font-family-special;
            font-size: 80%;
            text-transform: uppercase;
            letter-spacing: 0.15rem;
            border: 0;
        }
    }
}
</style>
