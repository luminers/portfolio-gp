<template>
  <main class="main-section">
    <Carrera />
    <Certificacion />
    <Front />

    <div class="back-tools">
      <h3 class="back">Back</h3>
      <h3>Tools</h3>
    </div>
    <div class="back-tools">
      <Back />

      <Tools />
    </div>
  </main>
</template>

<script>
import Carrera from "@/components/Carrera.vue";
import Certificacion from "@/components/FreeCodeCamp.vue";
import Front from "@/components/Front.vue";
import Back from "@/components/Back.vue";
import Tools from "@/components/Tools.vue";

export default {
  name: "ConocimientosComponente",
  components: {
    Carrera,
    Certificacion,
    Front,
    Back,
    Tools,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.main-section {
  width: 100%;
  height: auto;
  padding: 20px;
  display: flex;
  flex-flow: column wrap;
  font-size: 1em;
}

.div-content {
  display: flex;
  text-align: center;
  justify-content: center;
  align-items: center;
  padding: 12px 0px;
  height: auto;
  background: rgba(124, 124, 124, 0.129);
  box-shadow: 0 8px 32px 0 rgba(43, 43, 50, 0.37);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 5px;
  margin-bottom: 20px;
}
.carrera p {
  padding-left: 30px;
  margin-right: 1em;
}

.carrera-img {
  width: 200px;
}

.icon {
  width: 40px;
}

.icon-label {
  align-self: flex-end;
  font-weight: 600;
}

.front {
  padding: 10px;
  width: 70%;
  justify-content: space-evenly;
}
.back-tools {
  width: 100%;
  display: flex;
  flex-flow: row nowrap;
}

@media all and (max-width: 550px) {
  .div-content {
    width: 90%;
    padding-left: 50px;
  }
}
</style>
