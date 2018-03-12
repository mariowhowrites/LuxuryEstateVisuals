<template>
    <section class="absolute pin-t w-full h-full bg-black-fade text-white z-10">
        <p class="absolute pin-r pin-t mr-12 mt-2 text-5xl cursor-pointer" @click="destroyModal">X</p>
        <div class="w-full h-screen flex justify-center">
            <carousel/> 
        </div>
    </section>
</template>

<script>
import GalleryCarousel from "./GalleryCarousel"
import GallerySlide from "./GallerySlide"


export default {
  methods: {
      destroyModal() {
          console.log("destroying");
          this.$emit('toggle')
      }
  },
  components: {
      'carousel': GalleryCarousel, 
      'gallery-slide': GallerySlide
  }
}
</script>