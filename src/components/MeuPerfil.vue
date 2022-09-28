<template>
  <infoVue />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import infoVue from "./Perfil/info.vue";

export default defineComponent({
  name: "Meu Perfil",
  components: {
    infoVue,
  },
});
</script>

<style scoped>
h1 {
  color: purple;
}
</style>
