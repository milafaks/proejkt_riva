<template>
  <q-page padding>
    <div class="q-pa-md">
      <q-table
        title="Popis knjiga"
        :rows="rows"
        :columns="columns"
        row-key="id"
        flat
        bordered
        wrap-cells
      />
    </div>
  </q-page>
</template>

<script setup>
import { ref } from 'vue'

const columns = [
  {
    name: 'id',
    label: 'ID',
    field: 'id',
    align: 'left',
    sortable: true,
    style: { fontSize: '14px' },
    headerStyle: { fontSize: '18px', fontWeight: 'bold' }
  },
  {
    name: 'naslov',
    label: 'Naslov',
    field: 'naslov',
    align: 'left',
    sortable: true,
    style: { fontSize: '14px' },
    headerStyle: { fontSize: '18px', fontWeight: 'bold' }
  },
  {
    name: 'autor',
    label: 'Autor',
    field: 'autor',
    align: 'left',
    sortable: true,
    style: { fontSize: '14px' },
    headerStyle: { fontSize: '18px', fontWeight: 'bold' }
  },
  {
    name: 'opis',
    label: 'Opis',
    field: 'opis',
    align: 'left',
    style: { fontSize: '14px' },
    headerStyle: { fontSize: '18px', fontWeight: 'bold' }
  },
  {
    name: 'slika',
    label: 'Slika',
    field: 'slika',
    align: 'center',
    style: { fontSize: '14px' },
    headerStyle: { fontSize: '18px', fontWeight: 'bold' }
  },
  {
    name: 'status',
    label: 'Status',
    field: 'status',
    align: 'center',
    sortable: true,
    style: { fontSize: '14px' },
    headerStyle: { fontSize: '18px', fontWeight: 'bold' }
  }
]

const rows = ref([
  {
    id: 1,
    naslov: 'Na Drini ćuprija',
    autor: 'Ivo Andrić',
    opis: 'Roman o izgradnji mosta na Drini i sudbinama ljudi oko njega.',
    slika: '',
    status: 'slobodna'
  },
  {
    id: 2,
    naslov: 'Prokleta avlija',
    autor: 'Ivo Andrić',
    opis: 'Kratki roman o zatvoru i ljudskim sudbinama.',
    slika: '',
    status: 'zauzeta'
  },
  {
    id: 3,
    naslov: 'Zločin i kazna',
    autor: 'Fjodor Dostojevski',
    opis: 'Psihološki roman o krivnji i iskupljenju.',
    slika: '',
    status: 'slobodna'
  },
  {
    id: 4,
    naslov: 'Ana Karenjina',
    autor: 'Lav Tolstoj',
    opis: 'Roman o tragičnoj ljubavi i društvenim normama.',
    slika: '',
    status: 'zauzeta'
  },
  {
    id: 5,
    naslov: 'Kiklop',
    autor: 'Ranko Marinković',
    opis: 'Modernistički roman o intelektualcu uoči Drugog svjetskog rata.',
    slika: '',
    status: 'slobodna'
  }
])
</script>
