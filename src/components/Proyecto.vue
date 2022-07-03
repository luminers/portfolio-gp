<template>
  <div class="proyecto">
    <img class="proyecto-img" :src="img" alt="" />
    <h3>{{ title }}</h3>
    <a :href="link"
      ><input type="button" class="link-btn" value="Ver Proyecto"
    /></a>

    <div class="logos">
      <img
        class="logo"
        v-for="(logo, index) in logos"
        :key="index"
        :src="logo"
        alt="logo"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "ProyectoComponente",
  props: {
    link: String,
    img: String,
    title: String,
    logos: Array,
  },
};
</script>

<style scoped>
h3 {
  padding-top: 10px;
  color: #333333;
}
.link-btn {
  margin-top: 10px;
  background: none;
  border-radius: 10px;
  width: 30vw;
  border: 1px solid #333333;
}
.link-btn:hover {
  cursor: pointer;
  background-color: #6292b552;
  transition: 0.7s ease;
}

.proyecto {
  display: flex;
  flex-flow: column wrap;
  justify-content: center;
  align-items: center;
  margin: 20px;
  background: rgba(124, 124, 124, 0.129);
  box-shadow: 0 8px 32px 0 rgba(43, 43, 50, 0.37);
  backdrop-filter: blur(4px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
}

.proyecto-img {
  width: 40vw;
  border-radius: 10px 10px 0 0;
}

.logo {
  margin: 10px;
  width: 4vw;
}
</style>
