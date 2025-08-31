<template>
  <section
    id="experience"
    class="py-20 bg-gradient-to-b from-gray-900 to-gray-800 text-white px-6"
  >
    <!-- Título -->
    <h2 class="text-3xl md:text-5xl font-bold text-center mb-12">
      {{ $t('experience.title') }}
    </h2>

    <!-- Lista de experiencias -->
    <div class="max-w-5xl mx-auto space-y-8">
      <div
        v-for="(job, index) in experience"
        :key="index"
        class="bg-gray-700 p-6 rounded-2xl shadow-lg hover:shadow-xl transition"
      >
        <div class="flex flex-col md:flex-row md:items-center md:justify-between mb-4">
          <h3 class="text-xl font-semibold text-blue-400">
            {{ job.role }}
          </h3>
          <p class="text-sm text-gray-400">{{ job.period }}</p>
        </div>

        <p class="text-gray-300 mb-2">{{ job.company }}</p>

        <ul class="list-disc list-inside space-y-1 text-gray-400">
          <li v-for="(task, tIndex) in job.tasks" :key="tIndex">
            {{ task }}
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup>
const experience = [
  {
    role: 'Desarrollador Frontend',
    company: 'TechCorp',
    period: '2020 - 2022',
    tasks: [
      'Implementación de interfaces modernas con Vue y Tailwind.',
      'Optimización del rendimiento y accesibilidad web.',
      'Colaboración con equipos de backend para integración de APIs.',
    ],
  },
  {
    role: 'Ingeniero de Software',
    company: 'InnovateX',
    period: '2022 - Presente',
    tasks: [
      'Diseño de arquitecturas escalables en aplicaciones SPA.',
      'Automatización de procesos con CI/CD.',
      'Mentoría a desarrolladores junior.',
    ],
  },
]
</script>
