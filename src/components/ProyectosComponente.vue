<template>
  <main class="main-section">
    <Proyecto
      v-for="(proyecto, index) in proyectos"
      :key="index"
      :link="proyecto.link"
      :github="proyecto.github"
      :img="proyecto.img"
      :logos="proyecto.logo"
      :title="proyecto.title"
    />
  </main>
</template>

<script>
import Proyecto from "@/components/Proyecto.vue";

export default {
  name: "ProyectosComponente",
  data() {
    return {
      proyectos: [
        {
          link: "https://luminers.github.io/KainotoLandingPage/",
          github: "https://github.com/luminers/KainotoLandingPage",
          img: "https://luminers.github.io/KainotoLandingPage/assets/img/nosotros.jpg",
          logo: [
            "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png",
            "https://www.returngis.net/wp-content/uploads/2012/05/logo_CSS3.png",
            "https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png",
          ],
          title: "Maqueta Proyecto Kainoto",
        },
        {
          link: "https://luminers.github.io/WP-Api-SPA/",
          github: "https://github.com/luminers/WP-Api-SPA",
          img: "https://css-tricks.com/wp-content/uploads/2022/05/wp-patterns-featured-image.jpg",
          logo: [
            "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png",
            "https://www.returngis.net/wp-content/uploads/2012/05/logo_CSS3.png",
            "https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png",
          ],
          title: "Scrapper con WordPress API",
        },
        {
          link: "https://luminers.github.io/MarioBros/",
          github: "https://github.com/luminers/MarioBros",
          img: "https://i.ytimg.com/vi/zKZrHr4yDZc/maxresdefault.jpg",
          logo: [
            "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png",
            "https://blog.repl.it/images/kaboom/kaboom.png",
            "https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png",
          ],
          title: "Mario Bros",
        },
        {
          link: "https://luminers.github.io/Generador-contrasena/",
          github: "https://github.com/luminers/Generador-contrasena",
          img: "https://github.com/luminers/Generador-contrasena/blob/main/GeneradorContrasenas.PNG?raw=true",
          logo: [
            "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png",
            "https://www.returngis.net/wp-content/uploads/2012/05/logo_CSS3.png",
            "https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png",
          ],
          title: "Generador de contraseñas",
        },
        {
          link: "https://github.com/luminers/Simulador-Plazo-Fijo/tree/main/spf-vue",
          github:
            "https://github.com/luminers/Simulador-Plazo-Fijo/tree/main/spf-vue",
          img: "https://thelemabogados.pe/wp-content/uploads/2021/04/ac-asesores-empresariales-DIAN-Tasa-inter%C3%A9s-moratorio-liquidar-deudas.jpg",
          logo: [
            "https://vuejs.org//images/logo.png",
            "https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png",
            "https://www.returngis.net/wp-content/uploads/2012/05/logo_CSS3.png",
          ],
          title: "Simulador plazo fijo",
        },
      ],
    };
  },
  components: {
    Proyecto,
  },
};
</script>

<style scoped>
.main-section {
  height: 200vh;
  display: flex;
  flex-flow: row wrap;
  align-items: center;
}
</style>
