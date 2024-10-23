<template>
  <q-page class="flex flex-center">

    <tabelaHorarioAula></tabelaHorarioAula>

    <linhaDoTempo></linhaDoTempo>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import linhaDoTempo from 'components/TimeLine.vue'
import tabelaHorarioAula from 'src/components/TableTeach.vue'
export default defineComponent({
  name: 'IndexPage',
  components: {
    linhaDoTempo,
    tabelaHorarioAula
  }
})
</script>
