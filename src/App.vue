<template>
  <nav>
    <ul>
      <li><a href="#home">{{ $t('nav.home') }}</a></li>
      <li><a href="#studies">{{ $t('nav.studies') }}</a></li>
      <li><a href="#experience">{{ $t('nav.experience') }}</a></li>
      <li><a href="#certifications">{{ $t('nav.certifications') }}</a></li>
      <li><a href="#contact">{{ $t('nav.contact') }}</a></li>
    </ul>
    <select v-model="$i18n.locale">
      <option value="es">ES</option>
      <option value="en">EN</option>
    </select>
  </nav>
</template>
