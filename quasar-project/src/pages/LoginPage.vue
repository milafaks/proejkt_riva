<template>
  <q-page padding class="flex flex-center bg-grey-2">
    <q-card style="width: 100%; max-width: 400px;">
      <q-card-section class="bg-primary text-white">
        <div class="text-h6 text-center">Prijava</div>
      </q-card-section>

      <q-card-section>
        <q-input outlined v-model="username" label="Korisničko ime" />
        <q-input outlined v-model="password" type="password" label="Lozinka" class="q-mt-md" />
        <q-btn label="Potvrdi" color="primary" class="full-width q-mt-md" />
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const username = ref('')
const password = ref('')
</script>
