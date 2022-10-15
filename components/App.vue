<template>
    <div>
        <Navbar />
        <Main />
        <Footer />
    </div>
</template>

<script>
import Navbar from './Navbar.vue';
import Main from './Main.vue';
import Footer from './Footer.vue';
export default {
    name: "App",
    components: { Navbar, Main, Footer }
}
</script>