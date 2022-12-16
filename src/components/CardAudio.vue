<template>
  <div class="CardCustom">
    <template v-for="item in info" :key="item">
      <div class="card">
        <div class="left-part">
          <h2>{{item.title}}</h2>
          <p>{{item.author}}</p>
        </div>
        <audio id="yourAudio"
               controls
               controlsList="nodownload noplaybackrate"
            :src=item.mp3>
        </audio>
      </div>
    </template>
  </div>
</template>

<script>
import {ref} from "vue"

export default {
  name: 'CardCustom',

  props: {
    info: {}
  },

  setup() {


    const play = ref(false)

    return {play}
  }
}
</script>

<style scoped>

.card {
  display: grid;
  grid-template-columns: repeat(2, auto);
  gap: 10px;
  margin: 10px 0;
  padding: 15px;
  border: 1px solid #383838;
  border-radius: 15px;
  align-items: center;
  justify-content: start;
}

/* Specifies the size of the audio container */
audio {
  width: 115px;
  height: 25px;
}

audio::-webkit-media-controls-panel {
  -webkit-justify-content: center;
  height: 25px;
}

/* Removes the timeline */
audio::-webkit-media-controls-timeline {
  display: none !important;
}

/* Removes the time stamp */
audio::-webkit-media-controls-current-time-display {
  display: none;
}
audio::-webkit-media-controls-time-remaining-display {
  display: none;
}

audio::-webkit-media-controls-mute-button {
  display: none;
}

</style>
