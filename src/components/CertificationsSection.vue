<template>
  <section
    id="certifications"
    class="py-20 bg-gradient-to-b from-gray-800 to-gray-900 text-white px-6"
  >
    <!-- Título -->
    <h2 class="text-3xl md:text-5xl font-bold text-center mb-12">
      {{ $t('certifications.title') }}
    </h2>

    <!-- Lista de certificaciones -->
    <div class="max-w-5xl mx-auto grid gap-8 md:grid-cols-2">
      <div
        v-for="(cert, index) in certifications"
        :key="index"
        class="bg-gray-700 p-6 rounded-2xl shadow-lg hover:shadow-xl transition"
      >
        <h3 class="text-xl font-semibold text-blue-400 mb-2">
          {{ cert.name }}
        </h3>
        <p class="text-gray-300">{{ cert.issuer }}</p>
        <p class="text-sm text-gray-400 mb-4">{{ cert.year }}</p>

        <!-- Enlace opcional -->
        <a
          v-if="cert.link"
          :href="cert.link"
          target="_blank"
          rel="noopener noreferrer"
          class="text-blue-500 hover:underline text-sm"
        >
          {{ $t('certifications.verify') }}
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
const certifications = [
  {
    name: 'Microsoft Certified: Azure Fundamentals',
    issuer: 'Microsoft',
    year: '2024',
    link: 'https://learn.microsoft.com/en-us/users/danielmonederocabrera-2960/credentials/a8e2fc30af1815fc?ref=https%3A%2F%2Fwww.linkedin.com%2F',
  },
]
</script>
