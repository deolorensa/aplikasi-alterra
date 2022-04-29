<template>
  <div>
    <NavbarMain/>
    <div class="flex">
    <SidebarMain />
    <Nuxt />
    </div>
  </div>
</template>

<script>
import NavbarMain from "../components/NavbarMain.vue";
import SidebarMain from "../components/SidebarMain.vue";
export default {
    name: "IndexPage",
    components: { NavbarMain, SidebarMain, }
}
</script>