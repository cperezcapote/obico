<template>
    <header class="masthead">
        <div class="container d-flex h-100 align-items-center">
            <div class="mx-auto text-center">
                <img
                    class="logo img-fluid"
                    src="@/assets/img/logo.svg"
                    alt="O Bico Vermello"
                />
            </div>
        </div>
    </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "Header",
});
</script>

<style lang="scss" scoped>
@import "~@/assets/scss/styles.scss";

.masthead {
    position: relative;
    width: 100%;
    height: auto;
    min-height: 35rem;
    padding: 15rem 0;
    background: url("~@/assets/img/bg-masthead.jpg");
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: scroll;
    background-size: cover;
    h1 {
        font-family: $font-family-special;
        font-size: 2.5rem;
        line-height: 2.5rem;
        letter-spacing: 0.8rem;
        background: linear-gradient(fade-out($white, 0.1), fade-out($white, 1));
        -webkit-text-fill-color: transparent;
        background-clip: text;
    }
    h2 {
        max-width: 20rem;
        font-size: 1rem;
    }
    @include media-breakpoint-up(md) {
        h1 {
            font-size: 4rem;
            line-height: 4rem;
        }
    }
    .logo {
        width: 750px;
    }
    @include media-breakpoint-up(lg) {
        height: 100vh;
        padding: 0;
        h1 {
            font-size: 6.5rem;
            line-height: 6.5rem;
            letter-spacing: 0.8rem;
        }
        h2 {
            max-width: 30rem;
            font-size: 1.25rem;
        }
    }
}
</style>
