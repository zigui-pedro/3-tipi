<template>
  <div class="holder-info">
    <img
      src="https://img.freepik.com/premium-vector/mysterious-hacker-cat-cartoon_435121-75.jpg?size=500&ext=jpg"
      width="200"
      height="200"
    />
    <div class="info">
      <p class="nick">@{{ nickname }}</p>
      <p>
        Seguidores: {{ seguidores }} <br />
        Seguindo: {{ seguindo }}
      </p>
    </div>
    <div class="info2">
      <p>
        Publicações: {{ publicações }} <br />
        Curtidas: {{ curtidas }}
      </p>
    </div>
  </div>
  <div>
    <button @click="add()">Add seguidor</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Informações Perfil",
  data: () => {
    return {
      nickname: "3TIPI",
      seguidores: "3",
      seguindo: 1,
      publicações: 75,
      curtidas: 70000,
    };
  },
  /*methods: {
      add(){
          this.seguindo++;
      }
  }*/
});
</script>

<style scoped>
.holder-info {
  display: flex;
  height: 300px;
  background-image: url("https://wallpaperaccess.com/full/1113546.jpg");
  background-size: 100% 50%;
  background-repeat: no-repeat;
  background-color: /*#e4e4e4*/ lightgreen;
  padding-top: 120px;
  justify-content: space-evenly;
}

img {
  border-radius: 50%;
  margin: 20px;
}

.info {
  margin-top: 30px;
}

.info2 {
  margin-top: 60px;
}
/*
.info p:ntg-child(2){
    padding-bottom: 0px;
    margin-bottom: 0px;
}
*/
p {
  font-weight: bolder;
}

.nick {
  font-size: 16px;
}
</style>
