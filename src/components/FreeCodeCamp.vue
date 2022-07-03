<template>
  <div class="div-content">
    <p>
      Certificacion en "Responsive web desing" de FreeCodeCamp.org
      <a
        target="_blank"
        href="https://freecodecamp.org/certification/joaquinnu/responsive-web-design"
        ><input
          type="button"
          class="certificacion-btn"
          value="Ver Certificación"
      /></a>
    </p>

    <img
      class="fcc-img"
      src="https://design-style-guide.freecodecamp.org/downloads/fcc_secondary_small.png"
      alt="FCC logo"
    />
  </div>
</template>

<script>
export default {
  name: "FCCComponente",
};
</script>

<style scoped>
.div-content {
  padding: 20px;
}
.certificacion-btn {
  margin-top: 10px;
  background: none;
  border-radius: 10px;
  width: 70%;
  border: 1px solid #333333;
}
.certificacion-btn:hover {
  cursor: pointer;
  background-color: #6292b552;
  transition: 0.7s ease;
}
.fcc-img {
  margin-right: 2em;
  width: 6em;
}
</style>
