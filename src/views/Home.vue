<template>
    <div class="home">
        <NavBar />
        <Header />
        <Projects />
        <About />
        <SignUp />
        <Contact />
        <Footer />
    </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

import NavBar from "@/components/NavBar.vue";
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

import About from "@/components/sections/About.vue";
import Contact from "@/components/sections/Contact.vue";
import Projects from "@/components/sections/Projects.vue";
import SignUp from "@/components/sections/SignUp.vue";

export default defineComponent({
    name: "Home",
    components: {
        NavBar,
        Header,
        Footer,
        About,
        Contact,
        Projects,
        SignUp,
    },
});
</script>
