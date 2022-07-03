<template>
  <main class="main-section">
    <h3>Perfil</h3>
    <div class="div-content perfil">
      <p>
        Soy un estudiante universitario en busca de una oportunidad de trabajo
        que me permita crecer laboral y personalmente. Apasionado por la
        tecnología y la innovación, pero dispuesto a aprender sobre cualquier
        rubro. Cuento con una gran capacidad de aprendizaje y un gran sentido de
        responsabilidad.
      </p>
      <img class="img-perfil" :src="img" alt="foto" />
    </div>
    <h3>CV</h3>
    <div class="div-content cv">
      <iframe
        src="https://drive.google.com/file/d/1OzagDgdg-O3m0HWrhg1BU_LEQuvNcM4Q/preview"
        width="550"
        height="400"
      ></iframe>
    </div>
  </main>
</template>

<script>
export default {
  name: "ResumenComponente",
  data() {
    return {
      img: "https://github.com/luminers/portfolio-gp/blob/main/src/assets/perfil.png?raw=true",
    };
  },
};
</script>

<style scoped>
.main-section {
  height: 130vh;
  flex-flow: column nowrap;
  overflow-x: hidden;
  overflow: hidden;
}

.cv {
  width: 80vw;
  height: 80vh;
}

.perfil {
  padding: 0 5vw;
  margin: 0;
  width: 83vw;
  height: auto;
  margin-bottom: 20px;
}

.img-perfil {
  width: 30%;
  border-radius: 10px;
  margin: 10px;
}
</style>
