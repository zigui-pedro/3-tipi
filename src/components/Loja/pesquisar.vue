<template>
  <div class="holder-pesquisar">
    <ion-item class="input-pesquisar">
      <ion-input placeholder="Busque aqui seu produto"></ion-input>
      <ion-label class="label-pesquisar">
        <!-- 
            Aqui nos estamos utilizando uma tag chamada ion-icon 
            E a tag recebe um :icon que é o "search"
          -->
        <ion-icon :icon="search" />
      </ion-label>
    </ion-item>
  </div>
</template>

<script>
import { defineComponent } from "vue";

/**
 * O search foi importado aqui
 */
import { search } from "ionicons/icons";

export default defineComponent({
  name: "Pesquisar",
  setup() {
    /**
     * Foi inserido o search no meu codigo fonte
     */
    return {
      search,
    };
  },
});
</script>

<style>
.holder-pesquisar {
  width: 100%;
  height: 50px;
  background-color: #ffc200;
  padding-top: 10px;
}

.input-pesquisar {
  width: 60%;
  height: 30px;
  margin: auto;
  border-radius: 10px;
  border: 2px solid black;
}

.input-pesquisar input {
  margin-top: -20px;
}

.label-pesquisar {
  position: absolute;
  top: -5px;
  right: 5px;
  font-size: 26px;
}
</style>
