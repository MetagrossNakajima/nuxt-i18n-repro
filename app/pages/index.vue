<script setup>
const { locales, setLocale } = useI18n()
</script>

<template>
  <div>
    <button v-for="locale in locales" @click="setLocale(locale.code)">
      {{ locale.language }}
    </button>
    <h1>{{ $t("user.firstname") }}</h1>
  </div>
</template>
