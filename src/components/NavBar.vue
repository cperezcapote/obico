<template>
    <nav class="navbar navbar-expand-lg navbar-light fixed-top" id="mainNav">
        <div class="container">
            <a class="navbar-brand js-scroll-trigger" href="#page-top">
                O Bico Vermello
            </a>
            <button
                class="navbar-toggler navbar-toggler-right"
                type="button"
                data-toggle="collapse"
                data-target="#navbarResponsive"
                aria-controls="navbarResponsive"
                aria-expanded="false"
                aria-label="Toggle navigation"
            >
                Menu<i class="fas fa-bars"></i>
            </button>
            <div class="collapse navbar-collapse" id="navbarResponsive">
                <ul class="navbar-nav ml-auto">
                    <li class="nav-item">
                        <a class="nav-link js-scroll-trigger" href="#projects">
                            Products
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link js-scroll-trigger" href="#signup">
                            Contact
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "Navbar",
});
</script>

<style lang="scss" scoped>
@import "./src/assets/scss/styles.scss";

#mainNav {
    min-height: 3.5rem;
    background-color: $white;
    .navbar-toggler {
        font-size: 80%;
        padding: 0.75rem;
        color: $primary;
        border: $border-width solid $primary;
        &:focus {
            outline: none;
        }
    }
    .navbar-brand {
        color: $black;
        font-weight: 700;
        padding: 0.9rem 0;
    }
    .navbar-nav {
        .nav-item {
            &:hover {
                color: fade($white, 80%);
                outline: none;
                background-color: transparent;
            }
            &:active,
            &:focus {
                outline: none;
                background-color: transparent;
            }
        }
    }
    @include media-breakpoint-up(lg) {
        padding-top: 0;
        padding-bottom: 0;
        border-bottom: none;
        background-color: transparent;
        transition: background-color 0.3s ease-in-out;
        .navbar-brand {
            padding: 0.5rem 0;
            // color: fade-out($white, 0.5);
            color: $black;
        }
        .nav-link {
            transition: none;
            padding: 2rem 1.5rem;
            // color: fade-out($white, 0.5);
            color: $black;
            &:hover {
                // color: fade-out($white, 0.25);
                color: $black;
            }
            &:active {
                color: $white;
            }
        }
        &.navbar-shrink {
            background-color: $white;
            .navbar-brand {
                color: $black;
            }
            .nav-link {
                color: $black;
                padding: 1.5rem 1.5rem 1.25rem;
                border-bottom: 0.25rem solid transparent;
                &:hover {
                    color: $primary;
                }
                &:active {
                    color: darken($primary, 15%);
                }
                &.active {
                    color: $primary;
                    outline: none;
                    border-bottom: 0.25rem solid $primary;
                }
            }
        }
    }
}
</style>
