<template>
  <div class="font-sans flex flex-col items-center w-full relative">
    <gallery-modal v-if="modal" @toggle="toggleModal"/>
    <splash :toggleModal="toggleModal"/>    
    <info-bar/>
    <main-content/>
    <footer-map/>
  </div>
</template>

<script>
import GalleryModal from "~/components/GalleryModal.vue"
import Splash from "~/components/Splash.vue"
import InfoBar from "~/components/InfoBar.vue"
import MainContent from  "~/components/MainContent.vue"
import FooterMap from "~/components/FooterMap.vue"

export default {
  head: {
    title: 'Welcome',
    meta: [{ hid: 'description', name: 'description', content: 'Welcome' }]
  },
  data() {
    return {
      modal: false
    }
  },
  methods: {
    toggleModal() {
      this.modal = !this.modal;
    }
  },
  components: {
    'gallery-modal': GalleryModal,
    'splash': Splash,
    'info-bar': InfoBar,
    'main-content': MainContent,
    'footer-map': FooterMap,
  }
}
</script>

<style>

</style>

