<template>
  <div class="main-content flex justify-center bg-grey-lighter">
    <div class="w-3/5 flex">
        <main-content-body/>
        <main-content-sidebar/>
    </div>
  </div>
</template>

<script>
import MainContentBody from './MainContentBody.vue'
import MainContentSidebar from './MainContentSidebar.vue'

export default {
  components: {
    'main-content-body': MainContentBody,
    'main-content-sidebar': MainContentSidebar
  }
}
</script>
