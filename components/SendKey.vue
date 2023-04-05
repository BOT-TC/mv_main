<script setup lang="ts">
import { onMounted, watch, computed, ref } from 'vue'

const { keys, slide } = defineProps({
  keys: {
    default: 'home',
  },
  slide: {
    default: 0,
  },
})

const audio = ref() // https://www.w3schools.com/tags/ref_av_dom.asp
const currentTime = ref(0)
const paused = ref(false)
const showAudio = ref(false)
const runListener = ref(true)

const page = computed(() => {
  return $slidev.nav.currentPage
})

// const sendKeys = (myKeys) => {
//   if (currentTime.value > 3 && currentTime.value < 4) {
//     console.log('go to TOC')
//   }
//   if (currentTime.value > 6 && currentTime.value < 8) {
//     console.log('go to Home')
//   }
// }

onMounted(() => {

  // watch(audio?.value?.currentTime, (newTime, oldTime) => {
  //   console.log('time', newTime)
  // })

  //       window.dispatchEvent(new KeyboardEvent('keydown', { 'key': 't' }));
})

watch(page, (newSlide, oldSlide) => {
  console.log('slide', newSlide, oldSlide)
  console.log('audio', audio)
})

const play = () => {
  if (runListener.value) {
    setInterval(() => {
      if (audio.value.currentTime) {
        // sendKeys(keys);
        currentTime.value = audio.value.currentTime

        if (currentTime?.value > 3 && currentTime?.value < 4) {
          console.log('go to TOC ' + currentTime.value + " @@@@@@@@@@@@ " + $slidev.nav.currentPage)
          if ($slidev.nav.currentPage < 2) $slidev.nav.nextSlide();
        }
        if (currentTime?.value > 12 && currentTime?.value < 13) {
          console.log('go to Home' + currentTime.value + " @@@@@@@@@@@@ " + $slidev.nav.currentPage)
          if ($slidev.nav.currentPage < 3) $slidev.nav.nextSlide();
        }

        console.log('ref time', audio.value.currentTime)
      }
    }, 500);
    runListener.value = false;

  }
  audio.value.play();
}
const pauseSound = (): void => {
  audio.value.pause();
}

</script>

<template>
  <span>
    <button @click="play">( Begin )</button>
    <audio id="sound" ref="audio" xautoplay xcontrols>
      <source src="/audio/planet-earth-109360.mp3" type="audio/mpeg" />
    </audio>
  </span>
</template>
