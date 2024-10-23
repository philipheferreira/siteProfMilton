<template>
  <q-page class="flex flex-center">

    <div>

      <div class="q-px-lg q-py-md">

        <img alt="Quasar logo"
          src="https://www.unijui.edu.br/arquivos/tinyMCE4/comunica1/rotina%20de%20estudos%202023.png"
          style="height: 300px; width: 300px;" class="q-ma-md" />
        <p>Professor: Milton Nascimento</p>

      </div>

      <tabelaHorarioAula></tabelaHorarioAula>

      <linhaDoTempo></linhaDoTempo>

    </div>

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
