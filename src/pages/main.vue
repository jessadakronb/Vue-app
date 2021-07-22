<template>
  <div class="container">
    <manufacturer v-slot="data">
      <devices :manufacturerId="data.factId"></devices>
    </manufacturer>
  </div>
</template>


<script>
import Devices from "@/components/Devices.vue";
import Manufacturer from "@/components/Manufacturer.vue";
export default {
  name: "App",
  components: {
    Manufacturer: Manufacturer,
    Devices: Devices,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
