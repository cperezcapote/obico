<template>
    <section class="contact-section bg-black">
        <div class="container">
            <div class="row"></div>
            <div class="social d-flex justify-content-center">
                <a
                    class="mx-2"
                    href="https://www.facebook.com/O-Bico-Vermello-103354368386203"
                    ><i class="fab fa-facebook-f"></i></a
                ><a class="mx-2" href="https://www.instagram.com/obicovermello/"
                    ><i class="fab fa-instagram"></i
                ></a>
            </div>
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "Contact",
});
</script>

<style lang="scss" scoped>
@import "./src/assets/scss/styles.scss";

.contact-section {
    padding-top: 5rem;
    .card {
        border: 0;
        border-bottom: 0.25rem solid $primary;
        h4 {
            font-size: 0.8rem;
            font-family: $font-family-special;
            text-transform: uppercase;
            letter-spacing: 0.15rem;
        }
        hr {
            border-color: $primary;
            border-width: 0.25rem;
            width: 3rem;
        }
    }
    .social {
        margin-top: 5rem;
        a {
            text-align: center;
            height: 3rem;
            width: 3rem;
            background: fade-out($pink, 0.9);
            border-radius: 100%;
            line-height: 3rem;
            color: fade-out($pink, 0.2);
            &:hover {
                color: fade-out($pink, 0.5);
            }
            &:active {
                color: $pink;
            }
        }
    }
}
</style>
