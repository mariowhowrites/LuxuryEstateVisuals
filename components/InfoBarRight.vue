<template>
  <div class="info-bar-right flex-col w-1/3 p-4 border-r border-l leading-normal">
        <div class="flex justify-between py-1">
            <div class="label font-bold opacity-75">Property Type</div>
            <div class="value">{{ propertyType }}</div>
        </div>
        <div class="flex justify-between py-1">
            <div class="label font-bold opacity-75">Year Built</div>
            <div class="value">{{ yearBuilt }}</div>
        </div>
        <div class="flex justify-between py-1">
            <div class="label font-bold opacity-75">Lot Size</div>
            <div class="value">{{ lotSize }}</div>
        </div>
        <div class="flex justify-between py-1">
            <div class="label font-bold opacity-75">Stories</div>
            <div class="value">{{ stories }}</div>
        </div>
        <div class="flex justify-between py-1">
            <div class="label font-bold opacity-75">Garage</div>
            <div class="value">{{ garage }}</div>
        </div>
        <div class="flex justify-between py-1">
            <div class="label font-bold opacity-75">Parking Spaces</div>
            <div class="value">{{ parkingSpaces }}</div>
        </div>  
    </div>
</template>

<script>
export default {
  data() {
    return {
      propertyType: 'Single Family',
      yearBuilt: 2013,
      lotSize: '5,009 sf',
      stories: 3,
      garage: 'Detached',
      parkingSpaces: 6
    }
  }
}
</script>
