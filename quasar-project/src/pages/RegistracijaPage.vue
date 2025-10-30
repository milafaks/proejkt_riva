<template>
  <q-page padding class="flex flex-center bg-grey-2">
    <q-card style="width: 100%; max-width: 500px;">
      <q-card-section class="bg-primary text-white">
        <div class="text-h6 text-center">Registracija</div>
      </q-card-section>

      <q-card-section>
        <q-input outlined v-model="ime" label="Ime" />
        <q-input outlined v-model="prezime" label="Prezime" class="q-mt-md" />
        <q-input outlined v-model="email" label="Email" class="q-mt-md" />
        <q-input outlined v-model="korisnickoIme" label="Korisničko ime" class="q-mt-md" />
        <q-input outlined v-model="lozinka" type="password" label="Lozinka" class="q-mt-md" />
        <q-btn label="Potvrdi" color="primary" class="full-width q-mt-md" />
      </q-card-section>
    </q-card>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const ime = ref('')
const prezime = ref('')
const email = ref('')
const korisnickoIme = ref('')
const lozinka = ref('')
</script>
