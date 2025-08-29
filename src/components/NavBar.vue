<template>
  <nav class="fixed top-0 left-0 w-full bg-gray-900 bg-opacity-80 backdrop-blur-md shadow z-50">
    <div class="max-w-6xl mx-auto flex justify-between items-center p-4">
      <span class="text-xl font-bold text-white">Portfolio</span>

      <ul class="hidden md:flex space-x-6 text-gray-300">
        <li><a href="#home" class="hover:text-white">{{ $t('nav.home') }}</a></li>
        <li><a href="#studies" class="hover:text-white">{{ $t('nav.studies') }}</a></li>
        <li><a href="#experience" class="hover:text-white">{{ $t('nav.experience') }}</a></li>
        <li><a href="#certifications" class="hover:text-white">{{ $t('nav.certifications') }}</a></li>
        <li><a href="#contact" class="hover:text-white">{{ $t('nav.contact') }}</a></li>
      </ul>

      <select v-model="$i18n.locale" class="ml-4 px-2 py-1 rounded bg-gray-800 text-white border border-gray-700">
        <option value="es">ES</option>
        <option value="en">EN</option>
      </select>
    </div>
  </nav>
</template>
