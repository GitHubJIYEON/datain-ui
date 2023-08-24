<script setup>
import Header from "@/components/common/Header.vue";
import Footer from "@/components/common/Footer.vue";
</script>

<template>
    <Header />
    <main id="content">
        <router-view></router-view>
    </main>
    <!-- <Footer /> -->
</template>

<style scoped></style>
