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
            {{ $t(job.role) }}
          </h3>
          <p class="text-sm text-gray-400">{{ $t(job.period) }}</p>
        </div>

        <p class="text-gray-300 mb-2">{{ $t(job.company) }}</p>

        <ul class="list-disc list-inside space-y-1 text-gray-400">
          <li v-for="(task, tIndex) in job.tasks" :key="tIndex">
            {{ $t(task) }}
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script setup>
const experience = [
  {
    role: 'experience.items[0].role',
    company: 'experience.items[0].company',
    period: 'experience.items[0].period',
    tasks: [
      'experience.items[0].tasks[0]',
      'experience.items[0].tasks[1]',
      'experience.items[0].tasks[2]'
    ]
  },
  {
    role: 'experience.items[1].role',
    company: 'experience.items[1].company',
    period: 'experience.items[1].period',
    tasks: [
      'experience.items[1].tasks[0]',
      'experience.items[1].tasks[1]'
    ]
  },
  {
    role: 'experience.items[2].role',
    company: 'experience.items[2].company',
    period: 'experience.items[2].period',
    tasks: [
      'experience.items[2].tasks[0]',
      'experience.items[2].tasks[1]'
    ]
  }
]
</script>
