<template>
  <div>
    <Navbar />
    <main>
      <HeroSection />
      <StudiesSection />
      <ExperienceSection />
      <CertificationsSection />
      <ContactSection />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Navbar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import StudiesSection from './components/StudiesSection.vue'
import ExperienceSection from './components/ExperienceSection.vue'
import CertificationsSection from './components/CertificationsSection.vue'
import ContactSection from './components/ContactSection.vue'
import Footer from './components/Footer.vue'
</script>
