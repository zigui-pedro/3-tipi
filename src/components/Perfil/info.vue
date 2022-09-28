<template>
  <div class="holder-info" :style="`background-image: url(${imagens.capa})`">
    <img :src="imagens.perfil" width="140" height="140" />
    <div class="info">
      <p class="nickname">@{{ nickname }}</p>
      <p>
        Seguidores: {{ contador.seguidores }} <br />
        Seguindo: {{ contador.seguindo }}
      </p>
    </div>
    <div class="info-2">
      <p>
        Publicações: {{ contador.publicações }} <br />
        Curtidas: {{ contador.curtidas }}
      </p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Informações perfil",
  data: () => {
    return {
      nickname: "3TIPI",
      contador: {
        seguidores: 3000000,
        seguindo: 2,
        publicações: 75,
        curtidas: 70000,
      },
      imagens: {
        perfil:
          "https://img.freepik.com/premium-vector/mysterious-hacker-cat-cartoon_435121-75.jpg?w=2000",
        capa: "https://th.bing.com/th/id/R.9bc08c5447f0b5291390e12a22af03d9?rik=VKY4FyezikPG0Q&pid=ImgRaw&r=0",
      },
    };
  },
});
</script>

<style scoped>
.holder-info {
  display: flex;
  height: 300px;
  background-image: url("");
  background-size: 100% 50%;
  background-repeat: no-repeat;
  background-color: #e4e4e4;
  padding-top: 110px;
  justify-content: space-evenly;
}

img {
  border-radius: 50%;
  margin: 20px;
  box-shadow: 0px 8px 10px #888888;
}

.info {
  margin-top: 30px;
}

.info-2 {
  margin-top: 90px;
}

.nickname {
  font-size: 24px;
}

p {
  font-weight: bolder;
}
</style>
