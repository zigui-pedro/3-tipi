<template>
  <pesquisar />
</template>

<script lang="ts">
import { defineComponent } from "vue";
import pesquisar from "./Loja/pesquisar.vue";

export default defineComponent({
  name: "MinhaLoja",
  components: {
    pesquisar,
  },
});
</script>

<style scoped>
h1 {
  color: gold;
}
</style>
