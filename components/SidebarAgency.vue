<template>
<div class="sidebar-agency flex flex-col">
    <div class="bg-black agency flex flex-col items-center">
        <p class="text-lg uppercase py-2 ml-4 self-start text-white">PRESENTED BY</p>
        <img src="~/assets/lev-logo.jpg" alt="">
    </div>
    <div class="agent flex border-t border-b">
        <div class="agent-image w-1/3 min-h-ten-screen">
            <img src="~/assets/lev-agent.jpg" class="w-full h-full">
        </div>
        <div class="agent-contact w-2/3 flex pl-4 flex-col justify-center">
            <p class="text-lg uppercase">{{ name }}</p>
            <p class="italic text-sm pb-1">{{ agency }}</p>
            <p class="text-sm pb-1">{{ phone }}</p>
            <p class="text-sm pb-1">{{ email }}</p>
            <p class="text-sm">{{ licenseNumber }}</p>
        </div>
    </div>
    <div class="social-bar flex justify-around">
        
    </div>
</div>  
</template>

<script>
export default {
    data() {
        return {
            name: "Taylor Langius",
            agency: "Luxury Estate Visuals",
            phone: "(714) 504-0140",
            email: "taylorlangius@gmail.com",
            licenseNumber: "BRE# 8569A6D"
        }
    }
}
</script>

<style>
.bg-agent {
    background-image: url("~/assets/lev-agent.jpg");
}
</style>
