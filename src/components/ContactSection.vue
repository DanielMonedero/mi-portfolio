<template>
  <section
    id="contact"
    class="py-20 bg-gradient-to-b from-gray-900 to-gray-800 text-white px-6"
  >
    <!-- Título -->
    <h2 class="text-3xl md:text-5xl font-bold text-center mb-6">
      {{ $t('contact.title') }}
    </h2>

    <!-- Subtítulo -->
    <p class="text-center text-gray-300 max-w-2xl mx-auto mb-12">
      {{ $t('contact.subtitle') }}
    </p>

    <!-- Datos de contacto -->
    <div class="flex flex-col md:flex-row justify-center items-center gap-6 mb-12">
      <a
        href="mailto:danimc2002.dmc@gmail.com"
        class="px-6 py-3 bg-blue-600 rounded-full shadow-lg hover:bg-blue-500 transition duration-300"
      >
        {{ $t('contact.email') }}
      </a>
      <a
        href="https://www.linkedin.com/in/daniel-monedero-cabrera/"
        target="_blank"
        rel="noopener noreferrer"
        class="px-6 py-3 bg-gray-700 rounded-full shadow-lg hover:bg-gray-600 transition duration-300"
      >
        LinkedIn
      </a>
      <a
        href="https://github.com/DanielMonedero/"
        target="_blank"
        rel="noopener noreferrer"
        class="px-6 py-3 bg-gray-700 rounded-full shadow-lg hover:bg-gray-600 transition duration-300"
      >
        GitHub
      </a>
    </div>

    <!-- Formulario de contacto -->
    <form class="max-w-2xl mx-auto bg-gray-700 p-6 rounded-2xl shadow-lg space-y-4">
      <input
        type="text"
        placeholder="Nombre"
        class="w-full px-4 py-2 rounded-lg bg-gray-800 text-white border border-gray-600 focus:outline-none focus:ring-2 focus:ring-blue-500"
      />
      <input
        type="email"
        placeholder="Email"
        class="w-full px-4 py-2 rounded-lg bg-gray-800 text-white border border-gray-600 focus:outline-none focus:ring-2 focus:ring-blue-500"
      />
      <textarea
        placeholder="Mensaje"
        rows="5"
        class="w-full px-4 py-2 rounded-lg bg-gray-800 text-white border border-gray-600 focus:outline-none focus:ring-2 focus:ring-blue-500"
      ></textarea>
      <button
        type="submit"
        class="w-full px-6 py-3 bg-blue-600 rounded-full shadow-lg hover:bg-blue-500 transition duration-300"
      >
        {{ $t('contact.send') }}
      </button>
    </form>
  </section>
</template>

<script setup>
/* No requiere lógica por ahora.
   Si más adelante quieres enviar el formulario,
   se puede integrar con EmailJS, Formspree o tu propio backend. */
</script>
