
<template>
<section class="info-bar border-b w-full flex-col flex items-center">
    <div class="w-3/5 flex justify-between">
        <info-bar-left/>
        <info-bar-right/>
    </div>
</section>  
</template>

<script>
import InfoBarLeft from "./InfoBarLeft.vue"
import InfoBarRight from "./InfoBarRight.vue"

export default {
    components: {
        'info-bar-left': InfoBarLeft,
        'info-bar-right': InfoBarRight,
    }
}
</script>
