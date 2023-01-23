<script lang="ts">
import NavbarItem from "./components/NavbarItem.vue";
import FooterItem from "./components/FooterItem.vue";
export default {
  name: "App",
  components: {
    NavbarItem,
    FooterItem,
  },
}
</script>

<template>
  <div>
    <NavbarItem />
    <FooterItem />
    <router-view class="container" />
  </div>
</template>

<style>

</style>
