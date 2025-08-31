<template>
  <section
    id="home"
    class="flex flex-col items-center justify-center min-h-screen text-center bg-gradient-to-b from-gray-900 to-gray-800 text-white px-4"
  >
    <!-- Título -->
    <h1 class="text-4xl md:text-6xl font-extrabold mb-4">
      {{ $t('hero.title') }}
    </h1>

    <!-- Subtítulo -->
    <p class="text-lg md:text-2xl text-gray-300 mb-8">
      {{ $t('hero.subtitle') }}
    </p>

    <!-- Botón -->
    <a
      href="#contact"
      class="px-6 py-3 bg-blue-600 rounded-full shadow-lg hover:bg-blue-500 transition duration-300"
    >
      {{ $t('nav.contact') }}
    </a>
  </section>
</template>
