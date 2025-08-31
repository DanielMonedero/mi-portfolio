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
          {{ $t(study.degree) }}
        </h3>
        <p class="text-gray-300">{{ $t(study.institution) }}</p>
        <p class="text-sm text-gray-400">{{ $t(study.period) }}</p>
      </div>
    </div>
  </section>
</template>

<script setup>
const studies = [
  {
    degree: 'studies.items.degree1',
    institution: 'studies.items.institution1',
    period: 'studies.items.period1',
  },
  {
    degree: 'studies.items.degree2',
    institution: 'studies.items.institution2',
    period: 'studies.items.period2',
  },
  {
    degree: 'studies.items.degree3',
    institution: 'studies.items.institution3',
    period: 'studies.items.period3',
  },
]
</script>
