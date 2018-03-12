<template>
    <div class="main-content-body w-2/3">
        <body-description/>
        <body-video/>
        <body-amenities/>
    </div>
</template>

<script>
import BodyDescription from "./BodyDescription.vue"
import BodyVideo from "./BodyVideo.vue"
import BodyAmenities from  "./BodyAmenities.vue"

export default {
  components: {
      'body-description': BodyDescription,
      'body-video': BodyVideo,
      'body-amenities': BodyAmenities
  }
}
</script>
