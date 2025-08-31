<template>
  <footer
    class="bg-gradient-to-b from-gray-800 to-gray-900 text-gray-400 py-6 px-6"
  >
    <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center justify-between gap-4">
      <!-- Texto -->
      <p class="text-sm text-center md:text-left">
        © {{ new Date().getFullYear() }} {{ $t('footer.rights') }}
      </p>

      <!-- Links -->
      <div class="flex gap-6">
        <a
          href="mailto:danimc2002.dmc@gmail.com"
          class="hover:text-white transition"
        >
          Email
        </a>
        <a
          href="https://linkedin.com/in/tuusuario"
          target="_blank"
          rel="noopener noreferrer"
          class="hover:text-white transition"
        >
          LinkedIn
        </a>
        <a
          href="https://github.com/tuusuario"
          target="_blank"
          rel="noopener noreferrer"
          class="hover:text-white transition"
        >
          GitHub
        </a>
      </div>
    </div>
  </footer>
</template>

<script setup>
/* Nada de lógica por ahora, todo estático.
   El año se actualiza automáticamente con new Date().getFullYear(). */
</script>
