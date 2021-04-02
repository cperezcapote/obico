<template>
    <footer class="footer bg-black text-center text-white-50">
        <div class="container">
            Copyright ©<a href="#!">O Bico Vermello</a>2021
        </div>
    </footer>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
    name: "Footer",
});
</script>

<style lang="scss" scoped>
.footer {
    padding: 5rem 0;
}
</style>
