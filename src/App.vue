<template>
  <main class="font-sans text-gray-900 overflow-x-hidden">
    <HeroSection />
    <ProfileSection />
    <ContactSection />
    <EducationSection />
    <SkillsSection />
    <ExperienceSection />
    <Footer />
  </main>
</template>

<script setup>
import { onMounted } from 'vue'
import AOS from 'aos'
import 'aos/dist/aos.css'

import HeroSection from './components/HeroSection.vue'
import ProfileSection from './components/ProfileSection.vue'
import ContactSection from './components/ContactSection.vue'
import EducationSection from './components/EducationSection.vue'
import SkillsSection from './components/SkillsSection.vue'
import ExperienceSection from './components/ExperienceSection.vue'
import Footer from './components/Footer.vue'

onMounted(() => {
  AOS.init({
    duration: 1000,
    once: true,
  })
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');

body {
  font-family: 'Inter', sans-serif;
  background-color: #f9fafb;
  margin: 0;
}
</style>
