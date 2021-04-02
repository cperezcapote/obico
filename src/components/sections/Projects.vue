<template>
    <section class="projects-section bg-black" id="projects">
        <div class="container">
            <!-- Featured Project Row-->
            <!-- Project One Row-->
            <div class="row justify-content-center no-gutters mb-5 mb-lg-0">
                <div class="col-lg-6">
                    <img
                        class="img-fluid"
                        src="@/assets/img/demo-image-01.jpeg"
                        alt=""
                    />
                </div>
                <div class="col-lg-6">
                    <div class="bg-black text-center h-100 project">
                        <div class="d-flex h-100">
                            <div
                                class="project-text w-100 my-auto text-center text-lg-left"
                            >
                                <h4 class="text-white">Misty</h4>
                                <p class="mb-0 text-white-50">
                                    An example of where you can put an image of
                                    a project, or anything else, along with a
                                    description.
                                </p>
                                <hr class="d-none d-lg-block mb-0 ml-0" />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "Projects",
});
</script>

<style lang="scss" scoped>
@import "./src/assets/scss/styles.scss";

#projects {
    &.projects-section {
        padding: 10rem 0;
        .featured-text {
            padding: 2rem;
            @include media-breakpoint-up(lg) {
                padding: 0 0 0 2rem;
                border-left: 0.5rem solid $primary;
            }
        }
        .project-text {
            padding: 3rem;
            font-size: 90%;
            @include media-breakpoint-up(lg) {
                padding: 5rem;
                hr {
                    border-color: $primary;
                    border-width: 0.25rem;
                    width: 30%;
                }
            }
        }
    }
}
</style>
