<template>
  <main class="main-section">
    <h3>Perfil</h3>
    <div class="div-content perfil">
      <p>
        Soy un estudiante universitario avanzado en busca de una oportunidad de
        trabajo que me permita crecer laboral y personalmente. Apasionado por la
        tecnología y la innovación, pero dispuesto a aprender sobre cualquier
        rubro. Cuento con una gran capacidad de aprendizaje y un gran sentido de
        responsabilidad.
      </p>
    </div>
    <h3>CV</h3>
    <div class="div-content cv">
      
      <iframe src="https://drive.google.com/file/d/1ndCBObUz4vfLL_1tmKvJH8KzyyCYS_71/preview" width="640" height="480" allow="autoplay"></iframe>
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
  padding: 10px 5vw;
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
@media all and (max-width: 550px) {
  .div-content {
    width: 50%;
  }
}
</style>
