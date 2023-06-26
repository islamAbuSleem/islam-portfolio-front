<script setup>
import { ref } from 'vue'
const today = ref(new Date())
</script>
<template>
    <v-container>
        <span class="text-dark">
            Overview
        </span>
        <div class="about mx-7 mt-8">
            <h3 class="heading text-primary">
                About me
            </h3>
            <p class="text-dark mt-5 text-subtitle-1">

                I am a senior front-end developer with {{ today.getFullYear() - 2016 }} years of experience building
                responsive web applications using
                HTML, CSS, JavaScript, Vue, React, and other modern web technologies. I have worked for several companies in
                the
                tech industry.

                My expertise includes building complex user interfaces, optimizing website performance, and ensuring
                cross-browser compatibility. I am passionate about creating beautiful and functional web applications that
                provide an exceptional user experience.

            </p>
        </div>
        <div class="about mx-7 mt-8">
            <h3 class="heading text-primary">
                Latest Projects
            </h3>
            <p class="text-center font-weight-bold mt-15">list of projects . . .</p>
        </div>
    </v-container>
</template>