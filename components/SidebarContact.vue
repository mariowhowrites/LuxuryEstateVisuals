<template>
<section class="sidebar-contact">
    <div class="contact-title border-b">
        <p class="text-lg uppercase py-3 ml-4">GET IN TOUCH</p>
    </div>
    <div class="contact-form flex flex-col px-6 pt-4">
        <div class="half-input w-full flex justify-between pb-4">
            <div class="w-475">
                <input required placeholder="First*" type="text" class="pl-2 py-2 border rounded-sm w-full">
            </div>
            <div class="w-475">
                <input required placeholder="Last*" type="text" class="pl-2 py-2 border rounded-sm w-full">
            </div>
        </div>
        <div class="full-input w-full pb-4"><input required placeholder="Phone*" type="tel" class="pl-2 py-2 border rounded-sm w-full"></div>
        <div class="full-input w-full pb-4"><input placeholder="Email" type="email" class="pl-2 py-2 border rounded-sm w-full"></div>
        <div class="full-area-input w-full border rounded-sm mb-4"><textarea class="max-w-full pl-2" name="message" id="message" rows="10" cols="100">Your Message</textarea></div>
        <button class="border px-2 py-2 w-1/3 hover:bg-grey-lighter rounded-sm">Send Inquiry</button> 
    </div>
</section>
</template>

<script>
export default {
    
}
</script>
