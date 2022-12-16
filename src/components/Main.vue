<template>
  <div class="CustomMain">
    <CardAudio :info="audioStorage" />
  </div>
</template>

<script>

import CardAudio from '../components/CardAudio.vue'
import {audioStorage} from "@/storage/storage";

export default {
  name: 'CustomMain',
  components: {
    CardAudio
  },

  setup() {

    return {audioStorage}
  }
}
</script>

<style scoped>

.CustomMain {
  padding: 120px 20px 60px;
  max-width: 1200px;
  margin: 0 auto;
}

</style>
