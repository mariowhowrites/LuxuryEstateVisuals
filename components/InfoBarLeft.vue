<template>
    <div class="info-bar-left w-2/3 pb-4 flex flex-col justify-around">
        <div class="leading-normal">
            <h1 class="text-4xl">{{ streetAddress }}</h1>
            <p class="opacity-50 text-lg">{{ streetAddress }} | {{ city }}, {{ state }} {{ zip }}</p>
        </div>
        <div class="specs flex w-1/2">
            <div class="flex flex-col items-center mr-12">
                <BedIcon class="w-12 opacity-75 mb-2"/>
                <p>{{ beds }}</p>
            </div>
            <div class="flex flex-col items-center mr-12">
                <BathIcon class="w-12 opacity-75 mb-2"/>
                <p>{{ baths }}</p>
            </div>
            <div class="flex flex-col items-center">
                <BuildingIcon class="w-12 opacity-75 mb-2"/>
                <p>{{ squareFootage }}</p>
            </div>
        </div>
    </div>
</template>

<script>
import BedIcon from "~/assets/svg/005-bed.svg"
import BathIcon from "~/assets/svg/007-bathtub.svg"
import BuildingIcon from "~/assets/svg/002-building.svg"

export default {
  data() {
    return {
      streetAddress: '11631 Wallingsford Road',
      city: 'Rossmoor',
      state: 'CA',
      zip: 90720,
      beds: '3 beds',
      baths: '1.75 baths',
      squareFootage: '1,736 sqft'
    }
  },
  components: {
      BedIcon,
      BathIcon,
      BuildingIcon
  }
}
</script>
