<template>
  <label for="locale">Locale: </label>
  <select v-model="$i18n.locale" id="locale">
    <option v-for="locale in $i18n.availableLocales" :value="locale">{{ locale }}</option>
  </select>
</template>

<style scoped>
  label, select {
    width: 100%;
  }
  select {
    height: 25px;
  }
</style>