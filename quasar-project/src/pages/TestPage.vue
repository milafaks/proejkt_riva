<template>
  <q-page padding>
    <p v-for="item in days" :key="item">
      <button v-if="item == 'Ponedjeljak'">
        {{ item }} *
      </button>
      <button v-else>
        {{ item }}
      </button>
    </p>
  </q-page>
</template>

<script setup>
const days = [
  'Ponedjeljak',
  'Utorak',
  'Srijeda',
  'Četvrtak',
  'Petak',
  'Subota',
  'Nedjelja'
]
</script>

