<template>
  <div class="q-pa-md">
    <q-table class="my-sticky-header-column-table" flat bordered title="Horário aulas" :rows="rows" :columns="columns"
      row-key="name" virtual-scroll />
  </div>
</template>

<script>
const columns = [
  {
    name: 'name',
    required: true,
    label: 'Horarios/Dias',
    align: 'left',
    field: row => row.name,
    format: val => `${val}`,
    sortable: true
  },
  { name: 'segundaFeira', align: 'center', label: 'Segunda', field: 'segunda', sortable: true },
  { name: 'tercaFeira', align: 'center', label: 'Terça', field: 'terca', sortable: true },
  { name: 'quartaFeira', align: 'center', label: 'Quarta', field: 'quarta' },
  { name: 'quintaFeira', align: 'center', label: 'Quinta', field: 'quinta' },
  { name: 'sabado', align: 'center', label: 'Sexta', field: 'sexta' },
  { name: 'calcium', align: 'center', label: 'Sabado', field: 'sabado', sortable: true },
  { name: 'iron', align: 'center', label: 'Domingo', field: 'domingo', sortable: true }
]

const rows = [
  {
    name: '08:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '09:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '10:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '11:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '12:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '13:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '14:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '15:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '16:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '17:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '18:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '19:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '20:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  },
  {
    name: '21:00',
    segunda: '--',
    terca: '--',
    quarta: '--',
    quinta: '--',
    sexta: '--',
    sabado: '--',
    domingo: '--'
  }
]

export default {
  setup() {
    return {
      columns,
      rows
    }
  }
}
</script>

<style lang="sass">
.my-sticky-header-column-table
  /* height or max-height is important */
  max-height: 400px

  /* specifying max-width so the example can
    highlight the sticky column on any browser window */
  max-width: 900px
  width: auto

  td:first-child
    /* bg color is important for td; just specify one */
    background-color: #00b4ff

  tr th
    position: sticky
    /* higher than z-index for td below */
    z-index: 2
    /* bg color is important; just specify one */
    background: #00b4ff

  /* this will be the loading indicator */
  thead tr:last-child th
    /* height of all previous header rows */
    top: 48px
    /* highest z-index */
    z-index: 3
  thead tr:first-child th
    top: 0
    z-index: 1
  tr:first-child th:first-child
    /* highest z-index */
    z-index: 3

  td:first-child
    z-index: 1

  td:first-child, th:first-child
    position: sticky
    left: 0

  /* prevent scrolling behind sticky top row on focus */
  tbody
    /* height of all previous header rows */
    scroll-margin-top: 48px
</style>
