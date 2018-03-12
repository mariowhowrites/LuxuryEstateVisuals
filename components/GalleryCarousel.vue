<template>
  <div class="flex items-center">
    <p class="cursor-pointer text-5xl" @click="prev">&lt;</p>
        <transition name="up" mode="out-in">
            <gallery-slide v-cloak class="px-8" v-for="n in 11" v-if="n == index" :key="n" :iter="n"/>
        </transition>
    <p class="cursor-pointer text-5xl" @click="next">&gt;</p>
  </div>
</template>

<script>
import GallerySlide from './GallerySlide.vue'
export default {
  data() {
    return {
      index: 1
    }
  },
  methods: {
    next() {
      console.log(this.index)
      this.index = this.index === 11 ? 1 : this.index + 1
      console.log(this.index)
    },
    prev() {
      console.log(this.index)
      this.index = this.index === 1 ? 11 : this.index - 1
      console.log(this.index)
    }
  },
  components: {
    'gallery-slide': GallerySlide
  }
}
</script>

<style scoped>
.up-enter, .up-leave-to {
    transform: translateY(-20px);
    opacity: 0;
}

.up-leave-active, .up-enter-active {
    transition: all .4s ease-in-out;
}
</style>


