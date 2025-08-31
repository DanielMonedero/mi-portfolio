<template>
  <section
    id="studies"
    class="py-20 bg-gradient-to-b from-gray-800 to-gray-900 text-white px-6"
  >
    <!-- Título -->
    <h2 class="text-3xl md:text-5xl font-bold text-center mb-12">
      {{ $t('studies.title') }}
    </h2>

    <!-- Lista de estudios -->
    <div class="max-w-4xl mx-auto space-y-8">
      <div
        v-for="(study, index) in studies"
        :key="index"
        class="relative bg-gray-700 p-6 rounded-2xl shadow-lg hover:shadow-xl transition"
      >
        <h3 class="text-xl font-semibold text-blue-400 mb-2">
          {{ study.degree }}
        </h3>
        <p class="text-gray-300">{{ study.institution }}</p>
        <p class="text-sm text-gray-400">{{ study.period }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const studies = [
  {
    degree: 'Grado en Computación e Inteligencia Artificial',
    institution: 'Universidad Alfonso X el Sabio',
    period: 'Octubre 2024 - 2028',
  },
  {
    degree: 'Técnico Superior en Desarrollo de Aplicaciones Multiplataforma',
    institution: 'U-tad',
    period: 'Septiembre 2022 - Junio 2024',
  },
  {
    degree: 'Técnico en Sistemas Microinformáticos y Redes',
    institution: 'IES Los Cerros de Úbeda',
    period: 'Septiembre 2020 - Junio 2022',
  },
]
</script>
