<template>
    <img v-cloak :src="link" alt="">    
</template>

<script>

export default {
  props: ['iter'],
  computed: {
      number() {
          return ('0' + this.iter).slice(-2);
      },
      link() {
          return "/LuxuryEstateVisuals/slider/" + this.number + ".jpg";
      },
  }
}
</script>
