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
    role: 'Desarrollador de Software',
    company: 'Exceltic',
    period: 'Julio 2024 - Presente',
    tasks: [
      'Desarrollo desde cero de una app web completa.',
      'Backend con Java Spring Boot, Frontend con Vue.js 3.',
      'Integración con Oracle, Docker y Jenkins.'
    ],
  },
  {
    role: 'Desarrollador de Software (Prácticas)',
    company: 'Exceltic',
    period: 'Marzo 2024 - Junio 2024',
    tasks: [
      'Participación en proyectos de desarrollo web.',
      'Aprendizaje y colaboración con el equipo senior.'
    ],
  },
  {
    role: 'Técnico en Sistemas Microinformáticos y Redes',
    company: 'Datamac Informática',
    period: 'Septiembre 2021 - Junio 2022',
    tasks: [
      'Mantenimiento de sistemas y redes.',
      'Soporte técnico a usuarios.'
    ],
  },
]
</script>
