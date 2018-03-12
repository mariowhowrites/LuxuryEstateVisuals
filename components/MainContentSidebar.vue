<template>
  <div class="sidebar w-1/3 bg-white">
      <sidebar-agency/>
      <sidebar-contact/>
  </div>
</template>

<script>
import SidebarAgency from "./SidebarAgency.vue"
import SidebarContact from "./SidebarContact.vue"

export default {
  components: {
      'sidebar-agency': SidebarAgency,
      'sidebar-contact': SidebarContact
  }
}
</script>
