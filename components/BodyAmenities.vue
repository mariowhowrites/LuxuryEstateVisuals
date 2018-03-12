<template>
    <section class="amenities flex flex-wrap my-8">
      <div v-for="(amenity, key)  in amenities" :key="key" class="w-1/2 px-2 my-8">
        <ul class="list-reset amenity"><li class="text-center pl-4 relative">{{ amenity }}</li></ul>
      </div>  
    </section>
</template>

<script>
export default {
  data() {
    return {
      amenities: [
        "Cathedral-Vaulted Ceilings",
        "Zen Garden",
        "Unparalled Views",
        "Top Schools",
        "Storage Shed",
        "Rain Gutters",
      ]
    }
  }
}
</script>

<style>
.amenity li::before {
  position: absolute;
  left: 10%;
  top: 32%;
  content: "";
  margin-left: -1.3rem;
  display: inline-block;
  height: 1rem;
  width: 1rem;
  background-image: url("~/assets/check.png");
  background-size: contain;
  background-repeat: no-repeat;
}
</style>
