<template>
  <section class="flex flex-col items-center justify-center min-h-screen text-center bg-gradient-to-b from-gray-900 to-gray-800 text-white px-4">
    <h1 class="text-4xl md:text-6xl font-bold mb-4">
      {{ $t('hero.title', { name: 'Tu Nombre' }) }}
    </h1>
    <p class="text-lg md:text-2xl text-gray-300">
      {{ $t('hero.subtitle') }}
    </p>
    <a href="#contact" class="mt-6 px-6 py-3 bg-blue-600 rounded-full shadow-lg hover:bg-blue-500 transition">
      {{ $t('nav.contact') }}
    </a>
  </section>
</template>
