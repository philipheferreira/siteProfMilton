<template>
  <div class="tabela">
    <q-timeline :layout="layout" color="secondary">
      <q-timeline-entry heading>
        Linha do tempo Profissional
      </q-timeline-entry>

      <q-timeline-entry title="Início da Graduação em Licenciatura" subtitle="01 de janeiro de 2015" side="left">
      </q-timeline-entry>

      <q-timeline-entry title="Primeiras Turmas Particulares" subtitle="02 de janeiro de 2016" side="right">
        <div>
          Comecei a dar aulas particulares a alunos do ensino fundamental II
        </div>
      </q-timeline-entry>

      <!--<q-timeline-entry heading>November, 2017</q-timeline-entry> -->

      <q-timeline-entry title="Turmas do Ensino Médio" subtitle="02 de janeiro de 2017" side="left">
        <div>
          comecei a ministrar também aulas para alunos do ensino médio e participei de projeto de iniciação científica
        </div>
      </q-timeline-entry>

      <q-timeline-entry title="Projeto Análise" subtitle="02 de janeiro de 2018" side="right">
        <div>
          comecei a participar do projeto que viria a se chamar Análise e atendia alunos com objetivo de realizar a
          prova
          do ENEM e posteriormente trabalhamos preparando eles para procuras de concurso e mercado de trabalho e também
          apresentei artigo do COPAM (Congresso Panamazonico realizado na UFPA).
        </div>
      </q-timeline-entry>

      <q-timeline-entry title="Diploma em Licenciatura plena em Matemática" subtitle="02 de janeiro de 2019" side="left"
        color="orange" icon="done_all">
      </q-timeline-entry>

      <q-timeline-entry title="Event Title" subtitle="02 de janeiro de 2020" side="right">
        <div>
          aperfeiçoamento pessoal em matéria de religião com cursos de extensão da faculdade católica
        </div>
      </q-timeline-entry>

      <q-timeline-entry title="Event Title" subtitle="02 de janeiro de 2021" side="left">
        <div>
          Entendimento de que os problemas dos alunos passavam por não entender problemas matemáticos, traduzir para a
          linguagem matemática e montar um plano de resolução no qual soubessem descrever o porquê.
        </div>
      </q-timeline-entry>

      <q-timeline-entry title="EAM" subtitle="02 de janeiro de 2022" side="right">
        <div>
          Conheci a EAM (Experiência da Aprendizagem Mediada) elaborada por Reuven Feuerstein onde ele mostra os
          aspectos ambientais necessários para a educação e os métodos de mediação para ajudar o professor no auxilio
          da autonomia do aluno, desenvolvimento cognitivo.
        </div>
      </q-timeline-entry>

      <q-timeline-entry title="Teoria de Resolução de Problemas" subtitle="02 de janeiro de 2023" side="left">
        <div>
          Contato com a teoria RP (Resolução de Problemas) a qual deu uma resposta ao problema em que encontrei na
          dificuldade dos meus alunos em conseguir aprender a matemática e mostrou como torna-lá relevante para a
          vivência do aluno e um instrumento de desenvolvimento cognitivo, já que ela poderia reunir o que Reuven
          Feuerstein trabalha como necessário no desenvolvimento do aluno e a neurociência confirma.
        </div>
      </q-timeline-entry>
    </q-timeline>
  </div>
</template>

<script>
import { useQuasar } from 'quasar'
import { computed } from 'vue'

export default {
  setup() {
    const $q = useQuasar()

    return {
      layout: computed(() => {
        return $q.screen.lt.sm ? 'dense' : ($q.screen.lt.md ? 'comfortable' : 'loose')
      })
    }
  }
}
</script>
