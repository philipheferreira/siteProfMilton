<template>
  <q-page class="flex flex-center">
    <linhaDoTempo></linhaDoTempo>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import linhaDoTempo from 'components/TimeLine.vue'
export default defineComponent({
  name: 'IndexPage',
  components: {
    linhaDoTempo
  }
})
</script>
