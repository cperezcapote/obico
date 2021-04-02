<template>
    <section class="about-section text-center" id="about">
        <div class="container">
            <div class="row">
                <div class="col-lg-8 mx-auto">
                    <h2 class="text-white mb-4">Built with Bootstrap 4</h2>
                    <p class="text-white-50">
                        Grayscale is a free Bootstrap theme created by Start
                        Bootstrap. It can be yours right now, simply download
                        the template on<a
                            href="https://startbootstrap.com/theme/grayscale/"
                            >the preview page</a
                        >. The theme is open source, and you can use it for any
                        purpose, personal or commercial.
                    </p>
                </div>
            </div>
            <img class="img-fluid" src="assets/img/ipad.png" alt="" />
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "About",
});
</script>

<style lang="scss" scoped>
@import "./src/assets/scss/styles.scss";

.about-section {
    padding-top: 10rem;
    background: linear-gradient(
        to bottom,
        $black 0%,
        #{fade-out($black, 0.1)} 75%,
        #{fade-out($black, 0.2)} 100%
    );
    p {
        margin-bottom: 5rem;
    }
}
</style>
