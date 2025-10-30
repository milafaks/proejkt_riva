<template>
  <q-layout view="hHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn flat dense round icon="menu" aria-label="Menu" @click="toggleLeftDrawer" />

        <q-toolbar-title class="text-h1 text-green-8"> Plantie </q-toolbar-title>

        <div>Quasar v{{ $q.version }}</div>
      </q-toolbar>
    </q-header>

    <q-drawer v-model="leftDrawerOpen" show-if-above bordered>
      <q-list>
        <q-item-label header> Essential Links </q-item-label>

        <EssentialLink v-for="link in linksList" :key="link.title" v-bind="link" />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup>
import { ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'

const linksList = [
   {
    title: 'knjiznica-početna',
    caption: 'pocetna',
    icon: 'favorite',
    link: '#/',
  },
  {
    title: 'Docs',
    caption: 'quasar.dev',
    icon: 'school',
    link: 'https://quasar.dev',
  },
  {
    title: 'Github',
    caption: 'github.com/quasarframework',
    icon: 'code',
    link: 'https://github.com/quasarframework',
  },
  {
    title: 'Discord Chat Channel',
    caption: 'chat.quasar.dev',
    icon: 'chat',
    link: 'https://chat.quasar.dev',
  },
  {
    title: 'Forum',
    caption: 'forum.quasar.dev',
    icon: 'record_voice_over',
    link: 'https://forum.quasar.dev',
  },
  {
    title: 'Twitter',
    caption: '@quasarframework',
    icon: 'rss_feed',
    link: 'https://twitter.quasar.dev',
  },
  {
    title: 'Facebook',
    caption: '@QuasarFramework',
    icon: 'public',
    link: 'https://facebook.quasar.dev',
  },
  {
    title: 'Quasar Awesome',
    caption: 'Community Quasar projects',
    icon: 'favorite',
    link: 'https://awesome.quasar.dev',
  },
  {
    title: 'github projekt_riva',
    caption: 'proejkt_riva proejkt',
    icon: '',
    link: 'https://github.com/milafaks/proejkt_riva.git',
  },
  {
    title: 'knjiznica-nove knjige',
    caption: 'nove knjige',
    icon: 'favorite',
    link: '#/popisnovihknjiga',
  },
    {
    title: 'knjiznica-popis knjiga',
    caption: 'popis knjige',
    icon: 'favorite',
    link: '#/popisknjiga',
  },
    {
    title: 'Pretraživanje',
    caption: 'Pretraživanje',
    icon: 'favorite',
    link: '#/pretrazivanje',
  },
    {
    title: 'Lokacija',
    caption: 'Lokacija',
    icon: 'favorite',
    link: '#/lokacija',
  },
    {
    title: 'Login',
    caption: 'Login',
    icon: 'favorite',
    link: '#/login',
  },
    {
    title: 'Registracija',
    caption: 'Registracija',
    icon: 'favorite',
    link: '#/registracija',
  },

]

const leftDrawerOpen = ref(false)

function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value
}
</script>
