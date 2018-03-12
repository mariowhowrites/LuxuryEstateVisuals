<template>
<section class="splash relative flex items-end justify-center bg-photo bg-cover bg-center w-full h-half-screen">
    <div class="info-panel antialiased flex justify-between text-white text-lg text-bold  w-3/5">
        <div class="w-2/3 flex items-end">
          <div class="bg-black-fade rounded-t-sm mr-1 py-2 px-6">VIDEO TOUR</div>
          <div class="bg-black-fade rounded-t-sm py-2 px-6" @click="toggleModal">VIEW GALLERY</div>
        </div>
        <div class="w-1/3 flex items-end"><p class="w-full bg-black-fade rounded-t-sm pb-2 pt-1 pl-2 text-3xl">{{ price }}</p></div>
    </div>
</section>
</template>

<script>
import GalleryModal from "~/components/GalleryModal"

export default {
  props: ['toggleModal'],
  data() {
    return {
      price: "$1,078,324",
      modal: false
    }
  },
}
</script>

<style>
.bg-photo {
  background-image: url('~/assets/model-image-1.jpg');
}

.bg-black-fade {
  background-color: rgba(0, 0, 0, .75);
}
</style>
